# TemplateFox Go SDK

Official Go SDK for [TemplateFox](https://pdftemplateapi.com) - Generate PDFs from HTML templates via API.

[![Go Reference](https://pkg.go.dev/badge/github.com/TemplateFoxPDF/gosdk.svg)](https://pkg.go.dev/github.com/TemplateFoxPDF/gosdk)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## Installation

```bash
go get github.com/TemplateFoxPDF/gosdk
```

## Quick Start

```go
package main

import (
    "context"
    "fmt"
    "log"

    templatefox "github.com/TemplateFoxPDF/gosdk"
)

func main() {
    // Initialize the client
    config := templatefox.NewConfiguration()
    config.AddDefaultHeader("x-api-key", "your-api-key")

    client := templatefox.NewAPIClient(config)
    ctx := context.Background()

    // Generate a PDF
    request := templatefox.CreatePdfRequest{
        TemplateId: "YOUR_TEMPLATE_ID",
        Data: map[string]interface{}{
            "name":           "John Doe",
            "invoice_number": "INV-001",
            "total_amount":   150.00,
        },
    }

    response, _, err := client.PDFApi.CreatePdf(ctx, request)
    if err != nil {
        log.Fatal(err)
    }

    fmt.Printf("PDF URL: %s\n", *response.Url)
    fmt.Printf("Credits remaining: %d\n", *response.CreditsRemaining)
}
```

## Features

- **Template-based PDF generation** - Create templates with dynamic variables, generate PDFs with your data
- **Multiple export options** - Get a signed URL (default) or raw binary PDF
- **S3 integration** - Upload generated PDFs directly to your own S3-compatible storage
- **Context support** - Full context.Context support for cancellation and timeouts

## API Methods

### PDF Generation

```go
request := templatefox.CreatePdfRequest{
    TemplateId: "TEMPLATE_ID",
    Data: map[string]interface{}{
        "name": "John Doe",
    },
    ExportType: templatefox.PtrString("url"),  // "url" or "binary"
    Expiration: templatefox.PtrInt32(86400),   // URL expiration in seconds
    Filename:   templatefox.PtrString("invoice-001"),
}

response, _, err := client.PDFApi.CreatePdf(ctx, request)
```

### Templates

```go
// List all templates
templates, _, err := client.TemplatesApi.ListTemplates(ctx)
for _, t := range templates.Templates {
    fmt.Printf("%s: %s\n", t.Id, t.Name)
}

// Get template fields
fields, _, err := client.TemplatesApi.GetTemplateFields(ctx, "TEMPLATE_ID")
for _, f := range fields {
    fmt.Printf("%s: %s (required: %t)\n", f.Key, f.Type, f.Required)
}
```

### Account

```go
// Get account info
account, _, err := client.AccountApi.GetAccount(ctx)
fmt.Printf("Credits: %d\n", account.Credits)
fmt.Printf("Email: %s\n", *account.Email)

// List transactions (with optional params)
transactions, _, err := client.AccountApi.ListTransactions(ctx).
    Limit(100).
    Offset(0).
    Execute()
for _, tx := range transactions.Transactions {
    fmt.Printf("%s: %d credits\n", tx.TransactionType, tx.Credits)
}
```

### S3 Integration

```go
// Save S3 configuration
s3Config := templatefox.S3ConfigRequest{
    EndpointUrl:     "https://s3.amazonaws.com",
    AccessKeyId:     "AKIAIOSFODNN7EXAMPLE",
    SecretAccessKey: templatefox.PtrString("your-secret-key"),
    BucketName:      "my-pdf-bucket",
    DefaultPrefix:   templatefox.PtrString("generated/pdfs/"),
}

_, _, err := client.IntegrationsApi.SaveS3Config(ctx, s3Config)

// Test connection
test, _, err := client.IntegrationsApi.TestS3Connection(ctx)
fmt.Printf("Connection: %s\n", test.Message)
```

## Configuration

```go
config := templatefox.NewConfiguration()
config.Servers = templatefox.ServerConfigurations{
    {URL: "https://api.pdftemplateapi.com"},
}
config.AddDefaultHeader("x-api-key", os.Getenv("TEMPLATEFOX_API_KEY"))

client := templatefox.NewAPIClient(config)
```

## Error Handling

```go
response, httpResp, err := client.PDFApi.CreatePdf(ctx, request)

if err != nil {
    if httpResp != nil {
        switch httpResp.StatusCode {
        case 402:
            log.Println("Insufficient credits")
        case 403:
            log.Println("Access denied - check your API key")
        case 404:
            log.Println("Template not found")
        default:
            log.Printf("Error: %v", err)
        }
    } else {
        log.Printf("Error: %v", err)
    }
    return
}
```

## Documentation

- [API Documentation](https://pdftemplateapi.com/docs)
- [Swagger UI](https://api.pdftemplateapi.com/docs)
- [Dashboard](https://pdftemplateapi.com/dashboard)

## Support

- Email: support@pdftemplateapi.com
- Issues: [GitHub Issues](https://github.com/TemplateFoxPDF/gosdk/issues)

## License

MIT License - see [LICENSE](LICENSE) for details.

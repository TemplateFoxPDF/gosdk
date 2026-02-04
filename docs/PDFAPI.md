# \PDFAPI

All URIs are relative to *https://api.pdftemplateapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**CreatePdf**](PDFAPI.md#CreatePdf) | **Post** /v1/pdf/create | Generate PDF from template



## CreatePdf

> CreatePdfResponse CreatePdf(ctx).CreatePdfRequest(createPdfRequest).Execute()

Generate PDF from template



### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/TemplateFoxPDF/gosdk"
)

func main() {
	createPdfRequest := *openapiclient.NewCreatePdfRequest("TemplateId_example", map[string]interface{}{"key": interface{}(123)}) // CreatePdfRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.PDFAPI.CreatePdf(context.Background()).CreatePdfRequest(createPdfRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `PDFAPI.CreatePdf``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreatePdf`: CreatePdfResponse
	fmt.Fprintf(os.Stdout, "Response from `PDFAPI.CreatePdf`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreatePdfRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createPdfRequest** | [**CreatePdfRequest**](CreatePdfRequest.md) |  | 

### Return type

[**CreatePdfResponse**](CreatePdfResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json, application/pdf

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


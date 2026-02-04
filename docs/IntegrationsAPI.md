# \IntegrationsAPI

All URIs are relative to *https://api.pdftemplateapi.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**DeleteS3Config**](IntegrationsAPI.md#DeleteS3Config) | **Delete** /v1/integrations/s3 | Delete S3 configuration
[**GetS3Config**](IntegrationsAPI.md#GetS3Config) | **Get** /v1/integrations/s3 | Get S3 configuration
[**SaveS3Config**](IntegrationsAPI.md#SaveS3Config) | **Post** /v1/integrations/s3 | Save S3 configuration
[**TestS3Connection**](IntegrationsAPI.md#TestS3Connection) | **Post** /v1/integrations/s3/test | Test S3 connection



## DeleteS3Config

> S3SuccessResponse DeleteS3Config(ctx).Execute()

Delete S3 configuration



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.DeleteS3Config(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.DeleteS3Config``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `DeleteS3Config`: S3SuccessResponse
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.DeleteS3Config`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiDeleteS3ConfigRequest struct via the builder pattern


### Return type

[**S3SuccessResponse**](S3SuccessResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## GetS3Config

> S3ConfigResponse GetS3Config(ctx).Execute()

Get S3 configuration



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.GetS3Config(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.GetS3Config``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `GetS3Config`: S3ConfigResponse
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.GetS3Config`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiGetS3ConfigRequest struct via the builder pattern


### Return type

[**S3ConfigResponse**](S3ConfigResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## SaveS3Config

> S3SuccessResponse SaveS3Config(ctx).S3ConfigRequest(s3ConfigRequest).Execute()

Save S3 configuration



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
	s3ConfigRequest := *openapiclient.NewS3ConfigRequest("EndpointUrl_example", "AccessKeyId_example", "BucketName_example") // S3ConfigRequest | 

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.SaveS3Config(context.Background()).S3ConfigRequest(s3ConfigRequest).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.SaveS3Config``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `SaveS3Config`: S3SuccessResponse
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.SaveS3Config`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiSaveS3ConfigRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **s3ConfigRequest** | [**S3ConfigRequest**](S3ConfigRequest.md) |  | 

### Return type

[**S3SuccessResponse**](S3SuccessResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## TestS3Connection

> S3TestResponse TestS3Connection(ctx).Execute()

Test S3 connection



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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.IntegrationsAPI.TestS3Connection(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `IntegrationsAPI.TestS3Connection``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `TestS3Connection`: S3TestResponse
	fmt.Fprintf(os.Stdout, "Response from `IntegrationsAPI.TestS3Connection`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiTestS3ConnectionRequest struct via the builder pattern


### Return type

[**S3TestResponse**](S3TestResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


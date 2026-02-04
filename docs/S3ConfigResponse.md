# S3ConfigResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Configured** | **bool** | Whether S3 is configured | 
**EndpointUrl** | **string** | S3-compatible endpoint URL | 
**AccessKeyId** | **string** | Access key ID | 
**SecretAccessKeyMasked** | **string** | Masked secret access key (shows first 4 and last 4 characters) | 
**BucketName** | **string** | S3 bucket name | 
**DefaultPrefix** | **string** | Default path prefix for uploads | 

## Methods

### NewS3ConfigResponse

`func NewS3ConfigResponse(configured bool, endpointUrl string, accessKeyId string, secretAccessKeyMasked string, bucketName string, defaultPrefix string, ) *S3ConfigResponse`

NewS3ConfigResponse instantiates a new S3ConfigResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewS3ConfigResponseWithDefaults

`func NewS3ConfigResponseWithDefaults() *S3ConfigResponse`

NewS3ConfigResponseWithDefaults instantiates a new S3ConfigResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetConfigured

`func (o *S3ConfigResponse) GetConfigured() bool`

GetConfigured returns the Configured field if non-nil, zero value otherwise.

### GetConfiguredOk

`func (o *S3ConfigResponse) GetConfiguredOk() (*bool, bool)`

GetConfiguredOk returns a tuple with the Configured field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetConfigured

`func (o *S3ConfigResponse) SetConfigured(v bool)`

SetConfigured sets Configured field to given value.


### GetEndpointUrl

`func (o *S3ConfigResponse) GetEndpointUrl() string`

GetEndpointUrl returns the EndpointUrl field if non-nil, zero value otherwise.

### GetEndpointUrlOk

`func (o *S3ConfigResponse) GetEndpointUrlOk() (*string, bool)`

GetEndpointUrlOk returns a tuple with the EndpointUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpointUrl

`func (o *S3ConfigResponse) SetEndpointUrl(v string)`

SetEndpointUrl sets EndpointUrl field to given value.


### GetAccessKeyId

`func (o *S3ConfigResponse) GetAccessKeyId() string`

GetAccessKeyId returns the AccessKeyId field if non-nil, zero value otherwise.

### GetAccessKeyIdOk

`func (o *S3ConfigResponse) GetAccessKeyIdOk() (*string, bool)`

GetAccessKeyIdOk returns a tuple with the AccessKeyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessKeyId

`func (o *S3ConfigResponse) SetAccessKeyId(v string)`

SetAccessKeyId sets AccessKeyId field to given value.


### GetSecretAccessKeyMasked

`func (o *S3ConfigResponse) GetSecretAccessKeyMasked() string`

GetSecretAccessKeyMasked returns the SecretAccessKeyMasked field if non-nil, zero value otherwise.

### GetSecretAccessKeyMaskedOk

`func (o *S3ConfigResponse) GetSecretAccessKeyMaskedOk() (*string, bool)`

GetSecretAccessKeyMaskedOk returns a tuple with the SecretAccessKeyMasked field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecretAccessKeyMasked

`func (o *S3ConfigResponse) SetSecretAccessKeyMasked(v string)`

SetSecretAccessKeyMasked sets SecretAccessKeyMasked field to given value.


### GetBucketName

`func (o *S3ConfigResponse) GetBucketName() string`

GetBucketName returns the BucketName field if non-nil, zero value otherwise.

### GetBucketNameOk

`func (o *S3ConfigResponse) GetBucketNameOk() (*string, bool)`

GetBucketNameOk returns a tuple with the BucketName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketName

`func (o *S3ConfigResponse) SetBucketName(v string)`

SetBucketName sets BucketName field to given value.


### GetDefaultPrefix

`func (o *S3ConfigResponse) GetDefaultPrefix() string`

GetDefaultPrefix returns the DefaultPrefix field if non-nil, zero value otherwise.

### GetDefaultPrefixOk

`func (o *S3ConfigResponse) GetDefaultPrefixOk() (*string, bool)`

GetDefaultPrefixOk returns a tuple with the DefaultPrefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultPrefix

`func (o *S3ConfigResponse) SetDefaultPrefix(v string)`

SetDefaultPrefix sets DefaultPrefix field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



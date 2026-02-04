# S3ConfigRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**EndpointUrl** | **string** | S3-compatible endpoint URL. Must start with https:// | 
**AccessKeyId** | **string** | Access key ID for S3 authentication | 
**SecretAccessKey** | Pointer to **NullableString** |  | [optional] 
**BucketName** | **string** | S3 bucket name. Must follow S3 naming conventions (lowercase, no underscores) | 
**DefaultPrefix** | Pointer to **string** | Default path prefix for uploaded files. Can include slashes for folder structure | [optional] [default to ""]

## Methods

### NewS3ConfigRequest

`func NewS3ConfigRequest(endpointUrl string, accessKeyId string, bucketName string, ) *S3ConfigRequest`

NewS3ConfigRequest instantiates a new S3ConfigRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewS3ConfigRequestWithDefaults

`func NewS3ConfigRequestWithDefaults() *S3ConfigRequest`

NewS3ConfigRequestWithDefaults instantiates a new S3ConfigRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEndpointUrl

`func (o *S3ConfigRequest) GetEndpointUrl() string`

GetEndpointUrl returns the EndpointUrl field if non-nil, zero value otherwise.

### GetEndpointUrlOk

`func (o *S3ConfigRequest) GetEndpointUrlOk() (*string, bool)`

GetEndpointUrlOk returns a tuple with the EndpointUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndpointUrl

`func (o *S3ConfigRequest) SetEndpointUrl(v string)`

SetEndpointUrl sets EndpointUrl field to given value.


### GetAccessKeyId

`func (o *S3ConfigRequest) GetAccessKeyId() string`

GetAccessKeyId returns the AccessKeyId field if non-nil, zero value otherwise.

### GetAccessKeyIdOk

`func (o *S3ConfigRequest) GetAccessKeyIdOk() (*string, bool)`

GetAccessKeyIdOk returns a tuple with the AccessKeyId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAccessKeyId

`func (o *S3ConfigRequest) SetAccessKeyId(v string)`

SetAccessKeyId sets AccessKeyId field to given value.


### GetSecretAccessKey

`func (o *S3ConfigRequest) GetSecretAccessKey() string`

GetSecretAccessKey returns the SecretAccessKey field if non-nil, zero value otherwise.

### GetSecretAccessKeyOk

`func (o *S3ConfigRequest) GetSecretAccessKeyOk() (*string, bool)`

GetSecretAccessKeyOk returns a tuple with the SecretAccessKey field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecretAccessKey

`func (o *S3ConfigRequest) SetSecretAccessKey(v string)`

SetSecretAccessKey sets SecretAccessKey field to given value.

### HasSecretAccessKey

`func (o *S3ConfigRequest) HasSecretAccessKey() bool`

HasSecretAccessKey returns a boolean if a field has been set.

### SetSecretAccessKeyNil

`func (o *S3ConfigRequest) SetSecretAccessKeyNil(b bool)`

 SetSecretAccessKeyNil sets the value for SecretAccessKey to be an explicit nil

### UnsetSecretAccessKey
`func (o *S3ConfigRequest) UnsetSecretAccessKey()`

UnsetSecretAccessKey ensures that no value is present for SecretAccessKey, not even an explicit nil
### GetBucketName

`func (o *S3ConfigRequest) GetBucketName() string`

GetBucketName returns the BucketName field if non-nil, zero value otherwise.

### GetBucketNameOk

`func (o *S3ConfigRequest) GetBucketNameOk() (*string, bool)`

GetBucketNameOk returns a tuple with the BucketName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetBucketName

`func (o *S3ConfigRequest) SetBucketName(v string)`

SetBucketName sets BucketName field to given value.


### GetDefaultPrefix

`func (o *S3ConfigRequest) GetDefaultPrefix() string`

GetDefaultPrefix returns the DefaultPrefix field if non-nil, zero value otherwise.

### GetDefaultPrefixOk

`func (o *S3ConfigRequest) GetDefaultPrefixOk() (*string, bool)`

GetDefaultPrefixOk returns a tuple with the DefaultPrefix field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDefaultPrefix

`func (o *S3ConfigRequest) SetDefaultPrefix(v string)`

SetDefaultPrefix sets DefaultPrefix field to given value.

### HasDefaultPrefix

`func (o *S3ConfigRequest) HasDefaultPrefix() bool`

HasDefaultPrefix returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



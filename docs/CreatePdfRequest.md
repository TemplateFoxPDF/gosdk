# CreatePdfRequest

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TemplateId** | **string** | **Required.** Template short ID (12 characters) | 
**Data** | **map[string]interface{}** | **Required.** Key-value data to render in the template. Keys must match template variables. | 
**ExportType** | Pointer to [**ExportType**](ExportType.md) | Export format: &#x60;url&#x60; uploads to CDN and returns URL, &#x60;binary&#x60; returns raw PDF bytes | [optional] [default to URL]
**Expiration** | Pointer to **int32** | URL expiration in seconds. Min: 60 (1 min), Max: 604800 (7 days). Only applies to &#x60;url&#x60; export type. | [optional] [default to 86400]
**Filename** | Pointer to **NullableString** |  | [optional] 
**StoreS3** | Pointer to **bool** | Upload to your configured S3 bucket instead of CDN | [optional] [default to false]
**S3Filepath** | Pointer to **NullableString** |  | [optional] 
**S3Bucket** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewCreatePdfRequest

`func NewCreatePdfRequest(templateId string, data map[string]interface{}, ) *CreatePdfRequest`

NewCreatePdfRequest instantiates a new CreatePdfRequest object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePdfRequestWithDefaults

`func NewCreatePdfRequestWithDefaults() *CreatePdfRequest`

NewCreatePdfRequestWithDefaults instantiates a new CreatePdfRequest object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTemplateId

`func (o *CreatePdfRequest) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *CreatePdfRequest) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *CreatePdfRequest) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.


### GetData

`func (o *CreatePdfRequest) GetData() map[string]interface{}`

GetData returns the Data field if non-nil, zero value otherwise.

### GetDataOk

`func (o *CreatePdfRequest) GetDataOk() (*map[string]interface{}, bool)`

GetDataOk returns a tuple with the Data field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetData

`func (o *CreatePdfRequest) SetData(v map[string]interface{})`

SetData sets Data field to given value.


### GetExportType

`func (o *CreatePdfRequest) GetExportType() ExportType`

GetExportType returns the ExportType field if non-nil, zero value otherwise.

### GetExportTypeOk

`func (o *CreatePdfRequest) GetExportTypeOk() (*ExportType, bool)`

GetExportTypeOk returns a tuple with the ExportType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExportType

`func (o *CreatePdfRequest) SetExportType(v ExportType)`

SetExportType sets ExportType field to given value.

### HasExportType

`func (o *CreatePdfRequest) HasExportType() bool`

HasExportType returns a boolean if a field has been set.

### GetExpiration

`func (o *CreatePdfRequest) GetExpiration() int32`

GetExpiration returns the Expiration field if non-nil, zero value otherwise.

### GetExpirationOk

`func (o *CreatePdfRequest) GetExpirationOk() (*int32, bool)`

GetExpirationOk returns a tuple with the Expiration field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiration

`func (o *CreatePdfRequest) SetExpiration(v int32)`

SetExpiration sets Expiration field to given value.

### HasExpiration

`func (o *CreatePdfRequest) HasExpiration() bool`

HasExpiration returns a boolean if a field has been set.

### GetFilename

`func (o *CreatePdfRequest) GetFilename() string`

GetFilename returns the Filename field if non-nil, zero value otherwise.

### GetFilenameOk

`func (o *CreatePdfRequest) GetFilenameOk() (*string, bool)`

GetFilenameOk returns a tuple with the Filename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilename

`func (o *CreatePdfRequest) SetFilename(v string)`

SetFilename sets Filename field to given value.

### HasFilename

`func (o *CreatePdfRequest) HasFilename() bool`

HasFilename returns a boolean if a field has been set.

### SetFilenameNil

`func (o *CreatePdfRequest) SetFilenameNil(b bool)`

 SetFilenameNil sets the value for Filename to be an explicit nil

### UnsetFilename
`func (o *CreatePdfRequest) UnsetFilename()`

UnsetFilename ensures that no value is present for Filename, not even an explicit nil
### GetStoreS3

`func (o *CreatePdfRequest) GetStoreS3() bool`

GetStoreS3 returns the StoreS3 field if non-nil, zero value otherwise.

### GetStoreS3Ok

`func (o *CreatePdfRequest) GetStoreS3Ok() (*bool, bool)`

GetStoreS3Ok returns a tuple with the StoreS3 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStoreS3

`func (o *CreatePdfRequest) SetStoreS3(v bool)`

SetStoreS3 sets StoreS3 field to given value.

### HasStoreS3

`func (o *CreatePdfRequest) HasStoreS3() bool`

HasStoreS3 returns a boolean if a field has been set.

### GetS3Filepath

`func (o *CreatePdfRequest) GetS3Filepath() string`

GetS3Filepath returns the S3Filepath field if non-nil, zero value otherwise.

### GetS3FilepathOk

`func (o *CreatePdfRequest) GetS3FilepathOk() (*string, bool)`

GetS3FilepathOk returns a tuple with the S3Filepath field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetS3Filepath

`func (o *CreatePdfRequest) SetS3Filepath(v string)`

SetS3Filepath sets S3Filepath field to given value.

### HasS3Filepath

`func (o *CreatePdfRequest) HasS3Filepath() bool`

HasS3Filepath returns a boolean if a field has been set.

### SetS3FilepathNil

`func (o *CreatePdfRequest) SetS3FilepathNil(b bool)`

 SetS3FilepathNil sets the value for S3Filepath to be an explicit nil

### UnsetS3Filepath
`func (o *CreatePdfRequest) UnsetS3Filepath()`

UnsetS3Filepath ensures that no value is present for S3Filepath, not even an explicit nil
### GetS3Bucket

`func (o *CreatePdfRequest) GetS3Bucket() string`

GetS3Bucket returns the S3Bucket field if non-nil, zero value otherwise.

### GetS3BucketOk

`func (o *CreatePdfRequest) GetS3BucketOk() (*string, bool)`

GetS3BucketOk returns a tuple with the S3Bucket field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetS3Bucket

`func (o *CreatePdfRequest) SetS3Bucket(v string)`

SetS3Bucket sets S3Bucket field to given value.

### HasS3Bucket

`func (o *CreatePdfRequest) HasS3Bucket() bool`

HasS3Bucket returns a boolean if a field has been set.

### SetS3BucketNil

`func (o *CreatePdfRequest) SetS3BucketNil(b bool)`

 SetS3BucketNil sets the value for S3Bucket to be an explicit nil

### UnsetS3Bucket
`func (o *CreatePdfRequest) UnsetS3Bucket()`

UnsetS3Bucket ensures that no value is present for S3Bucket, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



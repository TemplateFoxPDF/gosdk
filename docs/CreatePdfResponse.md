# CreatePdfResponse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Url** | **string** | Signed URL to download the PDF (expires after specified time) | 
**Filename** | **string** | Filename of the generated PDF | 
**CreditsRemaining** | **int32** | Remaining credits after this request | 
**ExpiresIn** | **int32** | Seconds until URL expires | 

## Methods

### NewCreatePdfResponse

`func NewCreatePdfResponse(url string, filename string, creditsRemaining int32, expiresIn int32, ) *CreatePdfResponse`

NewCreatePdfResponse instantiates a new CreatePdfResponse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreatePdfResponseWithDefaults

`func NewCreatePdfResponseWithDefaults() *CreatePdfResponse`

NewCreatePdfResponseWithDefaults instantiates a new CreatePdfResponse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUrl

`func (o *CreatePdfResponse) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *CreatePdfResponse) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *CreatePdfResponse) SetUrl(v string)`

SetUrl sets Url field to given value.


### GetFilename

`func (o *CreatePdfResponse) GetFilename() string`

GetFilename returns the Filename field if non-nil, zero value otherwise.

### GetFilenameOk

`func (o *CreatePdfResponse) GetFilenameOk() (*string, bool)`

GetFilenameOk returns a tuple with the Filename field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFilename

`func (o *CreatePdfResponse) SetFilename(v string)`

SetFilename sets Filename field to given value.


### GetCreditsRemaining

`func (o *CreatePdfResponse) GetCreditsRemaining() int32`

GetCreditsRemaining returns the CreditsRemaining field if non-nil, zero value otherwise.

### GetCreditsRemainingOk

`func (o *CreatePdfResponse) GetCreditsRemainingOk() (*int32, bool)`

GetCreditsRemainingOk returns a tuple with the CreditsRemaining field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreditsRemaining

`func (o *CreatePdfResponse) SetCreditsRemaining(v int32)`

SetCreditsRemaining sets CreditsRemaining field to given value.


### GetExpiresIn

`func (o *CreatePdfResponse) GetExpiresIn() int32`

GetExpiresIn returns the ExpiresIn field if non-nil, zero value otherwise.

### GetExpiresInOk

`func (o *CreatePdfResponse) GetExpiresInOk() (*int32, bool)`

GetExpiresInOk returns a tuple with the ExpiresIn field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExpiresIn

`func (o *CreatePdfResponse) SetExpiresIn(v int32)`

SetExpiresIn sets ExpiresIn field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



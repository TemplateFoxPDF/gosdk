# TemplateField

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Key** | **string** | Field key/identifier | 
**Label** | **string** | Human-readable label | 
**Type** | Pointer to **string** | Field type: string, integer, number, boolean | [optional] [default to "string"]
**Required** | Pointer to **bool** | Whether the field is required | [optional] [default to false]
**HelpText** | Pointer to **NullableString** |  | [optional] 

## Methods

### NewTemplateField

`func NewTemplateField(key string, label string, ) *TemplateField`

NewTemplateField instantiates a new TemplateField object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTemplateFieldWithDefaults

`func NewTemplateFieldWithDefaults() *TemplateField`

NewTemplateFieldWithDefaults instantiates a new TemplateField object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetKey

`func (o *TemplateField) GetKey() string`

GetKey returns the Key field if non-nil, zero value otherwise.

### GetKeyOk

`func (o *TemplateField) GetKeyOk() (*string, bool)`

GetKeyOk returns a tuple with the Key field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetKey

`func (o *TemplateField) SetKey(v string)`

SetKey sets Key field to given value.


### GetLabel

`func (o *TemplateField) GetLabel() string`

GetLabel returns the Label field if non-nil, zero value otherwise.

### GetLabelOk

`func (o *TemplateField) GetLabelOk() (*string, bool)`

GetLabelOk returns a tuple with the Label field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLabel

`func (o *TemplateField) SetLabel(v string)`

SetLabel sets Label field to given value.


### GetType

`func (o *TemplateField) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *TemplateField) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *TemplateField) SetType(v string)`

SetType sets Type field to given value.

### HasType

`func (o *TemplateField) HasType() bool`

HasType returns a boolean if a field has been set.

### GetRequired

`func (o *TemplateField) GetRequired() bool`

GetRequired returns the Required field if non-nil, zero value otherwise.

### GetRequiredOk

`func (o *TemplateField) GetRequiredOk() (*bool, bool)`

GetRequiredOk returns a tuple with the Required field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRequired

`func (o *TemplateField) SetRequired(v bool)`

SetRequired sets Required field to given value.

### HasRequired

`func (o *TemplateField) HasRequired() bool`

HasRequired returns a boolean if a field has been set.

### GetHelpText

`func (o *TemplateField) GetHelpText() string`

GetHelpText returns the HelpText field if non-nil, zero value otherwise.

### GetHelpTextOk

`func (o *TemplateField) GetHelpTextOk() (*string, bool)`

GetHelpTextOk returns a tuple with the HelpText field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetHelpText

`func (o *TemplateField) SetHelpText(v string)`

SetHelpText sets HelpText field to given value.

### HasHelpText

`func (o *TemplateField) HasHelpText() bool`

HasHelpText returns a boolean if a field has been set.

### SetHelpTextNil

`func (o *TemplateField) SetHelpTextNil(b bool)`

 SetHelpTextNil sets the value for HelpText to be an explicit nil

### UnsetHelpText
`func (o *TemplateField) UnsetHelpText()`

UnsetHelpText ensures that no value is present for HelpText, not even an explicit nil

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Transaction

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TransactionRef** | **string** | Unique transaction reference (UUID) | 
**TransactionType** | **string** | Transaction type: PDFGEN, PURCHASE, REFUND, BONUS | 
**TemplateId** | Pointer to **NullableString** |  | [optional] 
**ExecTm** | Pointer to **NullableInt32** |  | [optional] 
**Credits** | **int32** | Credits consumed (positive) or added (negative) | 
**CreatedAt** | **string** | ISO 8601 timestamp | 

## Methods

### NewTransaction

`func NewTransaction(transactionRef string, transactionType string, credits int32, createdAt string, ) *Transaction`

NewTransaction instantiates a new Transaction object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewTransactionWithDefaults

`func NewTransactionWithDefaults() *Transaction`

NewTransactionWithDefaults instantiates a new Transaction object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTransactionRef

`func (o *Transaction) GetTransactionRef() string`

GetTransactionRef returns the TransactionRef field if non-nil, zero value otherwise.

### GetTransactionRefOk

`func (o *Transaction) GetTransactionRefOk() (*string, bool)`

GetTransactionRefOk returns a tuple with the TransactionRef field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionRef

`func (o *Transaction) SetTransactionRef(v string)`

SetTransactionRef sets TransactionRef field to given value.


### GetTransactionType

`func (o *Transaction) GetTransactionType() string`

GetTransactionType returns the TransactionType field if non-nil, zero value otherwise.

### GetTransactionTypeOk

`func (o *Transaction) GetTransactionTypeOk() (*string, bool)`

GetTransactionTypeOk returns a tuple with the TransactionType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTransactionType

`func (o *Transaction) SetTransactionType(v string)`

SetTransactionType sets TransactionType field to given value.


### GetTemplateId

`func (o *Transaction) GetTemplateId() string`

GetTemplateId returns the TemplateId field if non-nil, zero value otherwise.

### GetTemplateIdOk

`func (o *Transaction) GetTemplateIdOk() (*string, bool)`

GetTemplateIdOk returns a tuple with the TemplateId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTemplateId

`func (o *Transaction) SetTemplateId(v string)`

SetTemplateId sets TemplateId field to given value.

### HasTemplateId

`func (o *Transaction) HasTemplateId() bool`

HasTemplateId returns a boolean if a field has been set.

### SetTemplateIdNil

`func (o *Transaction) SetTemplateIdNil(b bool)`

 SetTemplateIdNil sets the value for TemplateId to be an explicit nil

### UnsetTemplateId
`func (o *Transaction) UnsetTemplateId()`

UnsetTemplateId ensures that no value is present for TemplateId, not even an explicit nil
### GetExecTm

`func (o *Transaction) GetExecTm() int32`

GetExecTm returns the ExecTm field if non-nil, zero value otherwise.

### GetExecTmOk

`func (o *Transaction) GetExecTmOk() (*int32, bool)`

GetExecTmOk returns a tuple with the ExecTm field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExecTm

`func (o *Transaction) SetExecTm(v int32)`

SetExecTm sets ExecTm field to given value.

### HasExecTm

`func (o *Transaction) HasExecTm() bool`

HasExecTm returns a boolean if a field has been set.

### SetExecTmNil

`func (o *Transaction) SetExecTmNil(b bool)`

 SetExecTmNil sets the value for ExecTm to be an explicit nil

### UnsetExecTm
`func (o *Transaction) UnsetExecTm()`

UnsetExecTm ensures that no value is present for ExecTm, not even an explicit nil
### GetCredits

`func (o *Transaction) GetCredits() int32`

GetCredits returns the Credits field if non-nil, zero value otherwise.

### GetCreditsOk

`func (o *Transaction) GetCreditsOk() (*int32, bool)`

GetCreditsOk returns a tuple with the Credits field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCredits

`func (o *Transaction) SetCredits(v int32)`

SetCredits sets Credits field to given value.


### GetCreatedAt

`func (o *Transaction) GetCreatedAt() string`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Transaction) GetCreatedAtOk() (*string, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Transaction) SetCreatedAt(v string)`

SetCreatedAt sets CreatedAt field to given value.



[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



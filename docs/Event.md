# Event

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Event** | Pointer to **map[string]interface{}** | Event data | [optional] 
**Completed** | Pointer to **bool** | Event was successfully send to target url | [optional] 
**Error** | Pointer to **string** | Optional error description | [optional] 
**IssuedAt** | Pointer to **string** | ISO Date String | [optional] 

## Methods

### NewEvent

`func NewEvent() *Event`

NewEvent instantiates a new Event object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewEventWithDefaults

`func NewEventWithDefaults() *Event`

NewEventWithDefaults instantiates a new Event object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEvent

`func (o *Event) GetEvent() map[string]interface{}`

GetEvent returns the Event field if non-nil, zero value otherwise.

### GetEventOk

`func (o *Event) GetEventOk() (*map[string]interface{}, bool)`

GetEventOk returns a tuple with the Event field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEvent

`func (o *Event) SetEvent(v map[string]interface{})`

SetEvent sets Event field to given value.

### HasEvent

`func (o *Event) HasEvent() bool`

HasEvent returns a boolean if a field has been set.

### GetCompleted

`func (o *Event) GetCompleted() bool`

GetCompleted returns the Completed field if non-nil, zero value otherwise.

### GetCompletedOk

`func (o *Event) GetCompletedOk() (*bool, bool)`

GetCompletedOk returns a tuple with the Completed field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompleted

`func (o *Event) SetCompleted(v bool)`

SetCompleted sets Completed field to given value.

### HasCompleted

`func (o *Event) HasCompleted() bool`

HasCompleted returns a boolean if a field has been set.

### GetError

`func (o *Event) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *Event) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *Event) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *Event) HasError() bool`

HasError returns a boolean if a field has been set.

### GetIssuedAt

`func (o *Event) GetIssuedAt() string`

GetIssuedAt returns the IssuedAt field if non-nil, zero value otherwise.

### GetIssuedAtOk

`func (o *Event) GetIssuedAtOk() (*string, bool)`

GetIssuedAtOk returns a tuple with the IssuedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIssuedAt

`func (o *Event) SetIssuedAt(v string)`

SetIssuedAt sets IssuedAt field to given value.

### HasIssuedAt

`func (o *Event) HasIssuedAt() bool`

HasIssuedAt returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



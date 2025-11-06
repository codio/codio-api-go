# RestrictedIPRange

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] [default to false]
**Range** | Pointer to **string** | Each ip from new line. Can specify IP or subnet. | [optional] 

## Methods

### NewRestrictedIPRange

`func NewRestrictedIPRange() *RestrictedIPRange`

NewRestrictedIPRange instantiates a new RestrictedIPRange object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewRestrictedIPRangeWithDefaults

`func NewRestrictedIPRangeWithDefaults() *RestrictedIPRange`

NewRestrictedIPRangeWithDefaults instantiates a new RestrictedIPRange object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *RestrictedIPRange) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *RestrictedIPRange) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *RestrictedIPRange) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *RestrictedIPRange) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetRange

`func (o *RestrictedIPRange) GetRange() string`

GetRange returns the Range field if non-nil, zero value otherwise.

### GetRangeOk

`func (o *RestrictedIPRange) GetRangeOk() (*string, bool)`

GetRangeOk returns a tuple with the Range field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRange

`func (o *RestrictedIPRange) SetRange(v string)`

SetRange sets Range field to given value.

### HasRange

`func (o *RestrictedIPRange) HasRange() bool`

HasRange returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



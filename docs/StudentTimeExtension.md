# StudentTimeExtension

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ExtendedDeadline** | Pointer to **int32** | Extended assignment deadline for student | [optional] 
**ExtendedTimeLimit** | Pointer to **int32** | Extended exam time limit for student | [optional] 

## Methods

### NewStudentTimeExtension

`func NewStudentTimeExtension() *StudentTimeExtension`

NewStudentTimeExtension instantiates a new StudentTimeExtension object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStudentTimeExtensionWithDefaults

`func NewStudentTimeExtensionWithDefaults() *StudentTimeExtension`

NewStudentTimeExtensionWithDefaults instantiates a new StudentTimeExtension object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetExtendedDeadline

`func (o *StudentTimeExtension) GetExtendedDeadline() int32`

GetExtendedDeadline returns the ExtendedDeadline field if non-nil, zero value otherwise.

### GetExtendedDeadlineOk

`func (o *StudentTimeExtension) GetExtendedDeadlineOk() (*int32, bool)`

GetExtendedDeadlineOk returns a tuple with the ExtendedDeadline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtendedDeadline

`func (o *StudentTimeExtension) SetExtendedDeadline(v int32)`

SetExtendedDeadline sets ExtendedDeadline field to given value.

### HasExtendedDeadline

`func (o *StudentTimeExtension) HasExtendedDeadline() bool`

HasExtendedDeadline returns a boolean if a field has been set.

### GetExtendedTimeLimit

`func (o *StudentTimeExtension) GetExtendedTimeLimit() int32`

GetExtendedTimeLimit returns the ExtendedTimeLimit field if non-nil, zero value otherwise.

### GetExtendedTimeLimitOk

`func (o *StudentTimeExtension) GetExtendedTimeLimitOk() (*int32, bool)`

GetExtendedTimeLimitOk returns a tuple with the ExtendedTimeLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtendedTimeLimit

`func (o *StudentTimeExtension) SetExtendedTimeLimit(v int32)`

SetExtendedTimeLimit sets ExtendedTimeLimit field to given value.

### HasExtendedTimeLimit

`func (o *StudentTimeExtension) HasExtendedTimeLimit() bool`

HasExtendedTimeLimit returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



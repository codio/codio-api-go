# AssignmentProgress

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**SecondsSpent** | Pointer to **int32** | Seconds spent in the assignment | [optional] 
**Grade** | Pointer to **int32** | Student grade | [optional] 
**Status** | Pointer to **string** | Assignment status | [optional] 
**CompletionDate** | Pointer to **string** | Assignment completion date, ISO Date String | [optional] 
**ExtendedTimeLimit** | Pointer to **int32** | Extended time limit | [optional] 
**ExtendedDeadline** | Pointer to **int32** | Extended deadline | [optional] 

## Methods

### NewAssignmentProgress

`func NewAssignmentProgress() *AssignmentProgress`

NewAssignmentProgress instantiates a new AssignmentProgress object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAssignmentProgressWithDefaults

`func NewAssignmentProgressWithDefaults() *AssignmentProgress`

NewAssignmentProgressWithDefaults instantiates a new AssignmentProgress object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetSecondsSpent

`func (o *AssignmentProgress) GetSecondsSpent() int32`

GetSecondsSpent returns the SecondsSpent field if non-nil, zero value otherwise.

### GetSecondsSpentOk

`func (o *AssignmentProgress) GetSecondsSpentOk() (*int32, bool)`

GetSecondsSpentOk returns a tuple with the SecondsSpent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondsSpent

`func (o *AssignmentProgress) SetSecondsSpent(v int32)`

SetSecondsSpent sets SecondsSpent field to given value.

### HasSecondsSpent

`func (o *AssignmentProgress) HasSecondsSpent() bool`

HasSecondsSpent returns a boolean if a field has been set.

### GetGrade

`func (o *AssignmentProgress) GetGrade() int32`

GetGrade returns the Grade field if non-nil, zero value otherwise.

### GetGradeOk

`func (o *AssignmentProgress) GetGradeOk() (*int32, bool)`

GetGradeOk returns a tuple with the Grade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrade

`func (o *AssignmentProgress) SetGrade(v int32)`

SetGrade sets Grade field to given value.

### HasGrade

`func (o *AssignmentProgress) HasGrade() bool`

HasGrade returns a boolean if a field has been set.

### GetStatus

`func (o *AssignmentProgress) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *AssignmentProgress) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *AssignmentProgress) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *AssignmentProgress) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetCompletionDate

`func (o *AssignmentProgress) GetCompletionDate() string`

GetCompletionDate returns the CompletionDate field if non-nil, zero value otherwise.

### GetCompletionDateOk

`func (o *AssignmentProgress) GetCompletionDateOk() (*string, bool)`

GetCompletionDateOk returns a tuple with the CompletionDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletionDate

`func (o *AssignmentProgress) SetCompletionDate(v string)`

SetCompletionDate sets CompletionDate field to given value.

### HasCompletionDate

`func (o *AssignmentProgress) HasCompletionDate() bool`

HasCompletionDate returns a boolean if a field has been set.

### GetExtendedTimeLimit

`func (o *AssignmentProgress) GetExtendedTimeLimit() int32`

GetExtendedTimeLimit returns the ExtendedTimeLimit field if non-nil, zero value otherwise.

### GetExtendedTimeLimitOk

`func (o *AssignmentProgress) GetExtendedTimeLimitOk() (*int32, bool)`

GetExtendedTimeLimitOk returns a tuple with the ExtendedTimeLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtendedTimeLimit

`func (o *AssignmentProgress) SetExtendedTimeLimit(v int32)`

SetExtendedTimeLimit sets ExtendedTimeLimit field to given value.

### HasExtendedTimeLimit

`func (o *AssignmentProgress) HasExtendedTimeLimit() bool`

HasExtendedTimeLimit returns a boolean if a field has been set.

### GetExtendedDeadline

`func (o *AssignmentProgress) GetExtendedDeadline() int32`

GetExtendedDeadline returns the ExtendedDeadline field if non-nil, zero value otherwise.

### GetExtendedDeadlineOk

`func (o *AssignmentProgress) GetExtendedDeadlineOk() (*int32, bool)`

GetExtendedDeadlineOk returns a tuple with the ExtendedDeadline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtendedDeadline

`func (o *AssignmentProgress) SetExtendedDeadline(v int32)`

SetExtendedDeadline sets ExtendedDeadline field to given value.

### HasExtendedDeadline

`func (o *AssignmentProgress) HasExtendedDeadline() bool`

HasExtendedDeadline returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



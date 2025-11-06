# StudentInformation

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**StudentId** | Pointer to **string** | Student identification | [optional] 
**StudentEmail** | Pointer to **string** | Student email if available | [optional] 
**StudentName** | Pointer to **string** | Student actual name | [optional] 
**SecondsSpent** | Pointer to **int32** | Seconds spent in the assignment | [optional] 
**Grade** | Pointer to **int32** | Optional assignment grade, 0-100 | [optional] 
**ExtraCredit** | Pointer to **int32** | Optional extra points | [optional] 
**Status** | Pointer to **string** | Assignment status: STARTED, NOT_STARTED, COMPLETED | [optional] 
**CompletionDate** | Pointer to **time.Time** | Assignment completion date, ISO Date String | [optional] 
**ExtendedDeadline** | Pointer to **int32** | Extended deadline | [optional] 
**ExtendedTimeLimit** | Pointer to **int32** | Extended time limit | [optional] 

## Methods

### NewStudentInformation

`func NewStudentInformation() *StudentInformation`

NewStudentInformation instantiates a new StudentInformation object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStudentInformationWithDefaults

`func NewStudentInformationWithDefaults() *StudentInformation`

NewStudentInformationWithDefaults instantiates a new StudentInformation object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetStudentId

`func (o *StudentInformation) GetStudentId() string`

GetStudentId returns the StudentId field if non-nil, zero value otherwise.

### GetStudentIdOk

`func (o *StudentInformation) GetStudentIdOk() (*string, bool)`

GetStudentIdOk returns a tuple with the StudentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStudentId

`func (o *StudentInformation) SetStudentId(v string)`

SetStudentId sets StudentId field to given value.

### HasStudentId

`func (o *StudentInformation) HasStudentId() bool`

HasStudentId returns a boolean if a field has been set.

### GetStudentEmail

`func (o *StudentInformation) GetStudentEmail() string`

GetStudentEmail returns the StudentEmail field if non-nil, zero value otherwise.

### GetStudentEmailOk

`func (o *StudentInformation) GetStudentEmailOk() (*string, bool)`

GetStudentEmailOk returns a tuple with the StudentEmail field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStudentEmail

`func (o *StudentInformation) SetStudentEmail(v string)`

SetStudentEmail sets StudentEmail field to given value.

### HasStudentEmail

`func (o *StudentInformation) HasStudentEmail() bool`

HasStudentEmail returns a boolean if a field has been set.

### GetStudentName

`func (o *StudentInformation) GetStudentName() string`

GetStudentName returns the StudentName field if non-nil, zero value otherwise.

### GetStudentNameOk

`func (o *StudentInformation) GetStudentNameOk() (*string, bool)`

GetStudentNameOk returns a tuple with the StudentName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStudentName

`func (o *StudentInformation) SetStudentName(v string)`

SetStudentName sets StudentName field to given value.

### HasStudentName

`func (o *StudentInformation) HasStudentName() bool`

HasStudentName returns a boolean if a field has been set.

### GetSecondsSpent

`func (o *StudentInformation) GetSecondsSpent() int32`

GetSecondsSpent returns the SecondsSpent field if non-nil, zero value otherwise.

### GetSecondsSpentOk

`func (o *StudentInformation) GetSecondsSpentOk() (*int32, bool)`

GetSecondsSpentOk returns a tuple with the SecondsSpent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSecondsSpent

`func (o *StudentInformation) SetSecondsSpent(v int32)`

SetSecondsSpent sets SecondsSpent field to given value.

### HasSecondsSpent

`func (o *StudentInformation) HasSecondsSpent() bool`

HasSecondsSpent returns a boolean if a field has been set.

### GetGrade

`func (o *StudentInformation) GetGrade() int32`

GetGrade returns the Grade field if non-nil, zero value otherwise.

### GetGradeOk

`func (o *StudentInformation) GetGradeOk() (*int32, bool)`

GetGradeOk returns a tuple with the Grade field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGrade

`func (o *StudentInformation) SetGrade(v int32)`

SetGrade sets Grade field to given value.

### HasGrade

`func (o *StudentInformation) HasGrade() bool`

HasGrade returns a boolean if a field has been set.

### GetExtraCredit

`func (o *StudentInformation) GetExtraCredit() int32`

GetExtraCredit returns the ExtraCredit field if non-nil, zero value otherwise.

### GetExtraCreditOk

`func (o *StudentInformation) GetExtraCreditOk() (*int32, bool)`

GetExtraCreditOk returns a tuple with the ExtraCredit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtraCredit

`func (o *StudentInformation) SetExtraCredit(v int32)`

SetExtraCredit sets ExtraCredit field to given value.

### HasExtraCredit

`func (o *StudentInformation) HasExtraCredit() bool`

HasExtraCredit returns a boolean if a field has been set.

### GetStatus

`func (o *StudentInformation) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *StudentInformation) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *StudentInformation) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *StudentInformation) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetCompletionDate

`func (o *StudentInformation) GetCompletionDate() time.Time`

GetCompletionDate returns the CompletionDate field if non-nil, zero value otherwise.

### GetCompletionDateOk

`func (o *StudentInformation) GetCompletionDateOk() (*time.Time, bool)`

GetCompletionDateOk returns a tuple with the CompletionDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCompletionDate

`func (o *StudentInformation) SetCompletionDate(v time.Time)`

SetCompletionDate sets CompletionDate field to given value.

### HasCompletionDate

`func (o *StudentInformation) HasCompletionDate() bool`

HasCompletionDate returns a boolean if a field has been set.

### GetExtendedDeadline

`func (o *StudentInformation) GetExtendedDeadline() int32`

GetExtendedDeadline returns the ExtendedDeadline field if non-nil, zero value otherwise.

### GetExtendedDeadlineOk

`func (o *StudentInformation) GetExtendedDeadlineOk() (*int32, bool)`

GetExtendedDeadlineOk returns a tuple with the ExtendedDeadline field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtendedDeadline

`func (o *StudentInformation) SetExtendedDeadline(v int32)`

SetExtendedDeadline sets ExtendedDeadline field to given value.

### HasExtendedDeadline

`func (o *StudentInformation) HasExtendedDeadline() bool`

HasExtendedDeadline returns a boolean if a field has been set.

### GetExtendedTimeLimit

`func (o *StudentInformation) GetExtendedTimeLimit() int32`

GetExtendedTimeLimit returns the ExtendedTimeLimit field if non-nil, zero value otherwise.

### GetExtendedTimeLimitOk

`func (o *StudentInformation) GetExtendedTimeLimitOk() (*int32, bool)`

GetExtendedTimeLimitOk returns a tuple with the ExtendedTimeLimit field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExtendedTimeLimit

`func (o *StudentInformation) SetExtendedTimeLimit(v int32)`

SetExtendedTimeLimit sets ExtendedTimeLimit field to given value.

### HasExtendedTimeLimit

`func (o *StudentInformation) HasExtendedTimeLimit() bool`

HasExtendedTimeLimit returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



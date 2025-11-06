# ExamMode

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TimedMode** | Pointer to [**TimedExamMode**](TimedExamMode.md) |  | [optional] 
**ShuffleQuestionsOrder** | Pointer to **bool** |  | [optional] 
**ForwardOnlyNavigation** | Pointer to **bool** |  | [optional] 
**SingleLogin** | Pointer to **bool** |  | [optional] 
**Authentication** | Pointer to **bool** |  | [optional] 
**RestrictedIPRange** | Pointer to [**RestrictedIPRange**](RestrictedIPRange.md) |  | [optional] 

## Methods

### NewExamMode

`func NewExamMode() *ExamMode`

NewExamMode instantiates a new ExamMode object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewExamModeWithDefaults

`func NewExamModeWithDefaults() *ExamMode`

NewExamModeWithDefaults instantiates a new ExamMode object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTimedMode

`func (o *ExamMode) GetTimedMode() TimedExamMode`

GetTimedMode returns the TimedMode field if non-nil, zero value otherwise.

### GetTimedModeOk

`func (o *ExamMode) GetTimedModeOk() (*TimedExamMode, bool)`

GetTimedModeOk returns a tuple with the TimedMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimedMode

`func (o *ExamMode) SetTimedMode(v TimedExamMode)`

SetTimedMode sets TimedMode field to given value.

### HasTimedMode

`func (o *ExamMode) HasTimedMode() bool`

HasTimedMode returns a boolean if a field has been set.

### GetShuffleQuestionsOrder

`func (o *ExamMode) GetShuffleQuestionsOrder() bool`

GetShuffleQuestionsOrder returns the ShuffleQuestionsOrder field if non-nil, zero value otherwise.

### GetShuffleQuestionsOrderOk

`func (o *ExamMode) GetShuffleQuestionsOrderOk() (*bool, bool)`

GetShuffleQuestionsOrderOk returns a tuple with the ShuffleQuestionsOrder field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShuffleQuestionsOrder

`func (o *ExamMode) SetShuffleQuestionsOrder(v bool)`

SetShuffleQuestionsOrder sets ShuffleQuestionsOrder field to given value.

### HasShuffleQuestionsOrder

`func (o *ExamMode) HasShuffleQuestionsOrder() bool`

HasShuffleQuestionsOrder returns a boolean if a field has been set.

### GetForwardOnlyNavigation

`func (o *ExamMode) GetForwardOnlyNavigation() bool`

GetForwardOnlyNavigation returns the ForwardOnlyNavigation field if non-nil, zero value otherwise.

### GetForwardOnlyNavigationOk

`func (o *ExamMode) GetForwardOnlyNavigationOk() (*bool, bool)`

GetForwardOnlyNavigationOk returns a tuple with the ForwardOnlyNavigation field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetForwardOnlyNavigation

`func (o *ExamMode) SetForwardOnlyNavigation(v bool)`

SetForwardOnlyNavigation sets ForwardOnlyNavigation field to given value.

### HasForwardOnlyNavigation

`func (o *ExamMode) HasForwardOnlyNavigation() bool`

HasForwardOnlyNavigation returns a boolean if a field has been set.

### GetSingleLogin

`func (o *ExamMode) GetSingleLogin() bool`

GetSingleLogin returns the SingleLogin field if non-nil, zero value otherwise.

### GetSingleLoginOk

`func (o *ExamMode) GetSingleLoginOk() (*bool, bool)`

GetSingleLoginOk returns a tuple with the SingleLogin field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSingleLogin

`func (o *ExamMode) SetSingleLogin(v bool)`

SetSingleLogin sets SingleLogin field to given value.

### HasSingleLogin

`func (o *ExamMode) HasSingleLogin() bool`

HasSingleLogin returns a boolean if a field has been set.

### GetAuthentication

`func (o *ExamMode) GetAuthentication() bool`

GetAuthentication returns the Authentication field if non-nil, zero value otherwise.

### GetAuthenticationOk

`func (o *ExamMode) GetAuthenticationOk() (*bool, bool)`

GetAuthenticationOk returns a tuple with the Authentication field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAuthentication

`func (o *ExamMode) SetAuthentication(v bool)`

SetAuthentication sets Authentication field to given value.

### HasAuthentication

`func (o *ExamMode) HasAuthentication() bool`

HasAuthentication returns a boolean if a field has been set.

### GetRestrictedIPRange

`func (o *ExamMode) GetRestrictedIPRange() RestrictedIPRange`

GetRestrictedIPRange returns the RestrictedIPRange field if non-nil, zero value otherwise.

### GetRestrictedIPRangeOk

`func (o *ExamMode) GetRestrictedIPRangeOk() (*RestrictedIPRange, bool)`

GetRestrictedIPRangeOk returns a tuple with the RestrictedIPRange field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetRestrictedIPRange

`func (o *ExamMode) SetRestrictedIPRange(v RestrictedIPRange)`

SetRestrictedIPRange sets RestrictedIPRange field to given value.

### HasRestrictedIPRange

`func (o *ExamMode) HasRestrictedIPRange() bool`

HasRestrictedIPRange returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



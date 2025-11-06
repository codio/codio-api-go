# AssignmentSettingsResult

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**IsDisabled** | Pointer to **bool** |  | [optional] 
**ReleaseGrades** | Pointer to **bool** |  | [optional] 
**EnableResetAssignmentByStudent** | Pointer to **bool** |  | [optional] 
**DisableDownloadByStudent** | Pointer to **bool** |  | [optional] 
**VisibilityOnDisabled** | Pointer to **string** | Assignment visibility | [optional] 
**VisibilityOnCompleted** | Pointer to **string** | Assignment visibility on completed | [optional] 
**PenaltiesV2** | Pointer to [**PenaltySettings**](PenaltySettings.md) |  | [optional] 
**StartTime** | Pointer to **string** |  | [optional] 
**DueTime** | Pointer to **string** |  | [optional] 
**MarkAsCompleteOnDueDate** | Pointer to **bool** |  | [optional] 
**EndTime** | Pointer to **string** |  | [optional] 
**Action** | Pointer to **string** | Assignment action on completed | [optional] 
**ExamMode** | Pointer to [**ExamMode**](ExamMode.md) |  | [optional] 

## Methods

### NewAssignmentSettingsResult

`func NewAssignmentSettingsResult() *AssignmentSettingsResult`

NewAssignmentSettingsResult instantiates a new AssignmentSettingsResult object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAssignmentSettingsResultWithDefaults

`func NewAssignmentSettingsResultWithDefaults() *AssignmentSettingsResult`

NewAssignmentSettingsResultWithDefaults instantiates a new AssignmentSettingsResult object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIsDisabled

`func (o *AssignmentSettingsResult) GetIsDisabled() bool`

GetIsDisabled returns the IsDisabled field if non-nil, zero value otherwise.

### GetIsDisabledOk

`func (o *AssignmentSettingsResult) GetIsDisabledOk() (*bool, bool)`

GetIsDisabledOk returns a tuple with the IsDisabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDisabled

`func (o *AssignmentSettingsResult) SetIsDisabled(v bool)`

SetIsDisabled sets IsDisabled field to given value.

### HasIsDisabled

`func (o *AssignmentSettingsResult) HasIsDisabled() bool`

HasIsDisabled returns a boolean if a field has been set.

### GetReleaseGrades

`func (o *AssignmentSettingsResult) GetReleaseGrades() bool`

GetReleaseGrades returns the ReleaseGrades field if non-nil, zero value otherwise.

### GetReleaseGradesOk

`func (o *AssignmentSettingsResult) GetReleaseGradesOk() (*bool, bool)`

GetReleaseGradesOk returns a tuple with the ReleaseGrades field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReleaseGrades

`func (o *AssignmentSettingsResult) SetReleaseGrades(v bool)`

SetReleaseGrades sets ReleaseGrades field to given value.

### HasReleaseGrades

`func (o *AssignmentSettingsResult) HasReleaseGrades() bool`

HasReleaseGrades returns a boolean if a field has been set.

### GetEnableResetAssignmentByStudent

`func (o *AssignmentSettingsResult) GetEnableResetAssignmentByStudent() bool`

GetEnableResetAssignmentByStudent returns the EnableResetAssignmentByStudent field if non-nil, zero value otherwise.

### GetEnableResetAssignmentByStudentOk

`func (o *AssignmentSettingsResult) GetEnableResetAssignmentByStudentOk() (*bool, bool)`

GetEnableResetAssignmentByStudentOk returns a tuple with the EnableResetAssignmentByStudent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnableResetAssignmentByStudent

`func (o *AssignmentSettingsResult) SetEnableResetAssignmentByStudent(v bool)`

SetEnableResetAssignmentByStudent sets EnableResetAssignmentByStudent field to given value.

### HasEnableResetAssignmentByStudent

`func (o *AssignmentSettingsResult) HasEnableResetAssignmentByStudent() bool`

HasEnableResetAssignmentByStudent returns a boolean if a field has been set.

### GetDisableDownloadByStudent

`func (o *AssignmentSettingsResult) GetDisableDownloadByStudent() bool`

GetDisableDownloadByStudent returns the DisableDownloadByStudent field if non-nil, zero value otherwise.

### GetDisableDownloadByStudentOk

`func (o *AssignmentSettingsResult) GetDisableDownloadByStudentOk() (*bool, bool)`

GetDisableDownloadByStudentOk returns a tuple with the DisableDownloadByStudent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisableDownloadByStudent

`func (o *AssignmentSettingsResult) SetDisableDownloadByStudent(v bool)`

SetDisableDownloadByStudent sets DisableDownloadByStudent field to given value.

### HasDisableDownloadByStudent

`func (o *AssignmentSettingsResult) HasDisableDownloadByStudent() bool`

HasDisableDownloadByStudent returns a boolean if a field has been set.

### GetVisibilityOnDisabled

`func (o *AssignmentSettingsResult) GetVisibilityOnDisabled() string`

GetVisibilityOnDisabled returns the VisibilityOnDisabled field if non-nil, zero value otherwise.

### GetVisibilityOnDisabledOk

`func (o *AssignmentSettingsResult) GetVisibilityOnDisabledOk() (*string, bool)`

GetVisibilityOnDisabledOk returns a tuple with the VisibilityOnDisabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibilityOnDisabled

`func (o *AssignmentSettingsResult) SetVisibilityOnDisabled(v string)`

SetVisibilityOnDisabled sets VisibilityOnDisabled field to given value.

### HasVisibilityOnDisabled

`func (o *AssignmentSettingsResult) HasVisibilityOnDisabled() bool`

HasVisibilityOnDisabled returns a boolean if a field has been set.

### GetVisibilityOnCompleted

`func (o *AssignmentSettingsResult) GetVisibilityOnCompleted() string`

GetVisibilityOnCompleted returns the VisibilityOnCompleted field if non-nil, zero value otherwise.

### GetVisibilityOnCompletedOk

`func (o *AssignmentSettingsResult) GetVisibilityOnCompletedOk() (*string, bool)`

GetVisibilityOnCompletedOk returns a tuple with the VisibilityOnCompleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibilityOnCompleted

`func (o *AssignmentSettingsResult) SetVisibilityOnCompleted(v string)`

SetVisibilityOnCompleted sets VisibilityOnCompleted field to given value.

### HasVisibilityOnCompleted

`func (o *AssignmentSettingsResult) HasVisibilityOnCompleted() bool`

HasVisibilityOnCompleted returns a boolean if a field has been set.

### GetPenaltiesV2

`func (o *AssignmentSettingsResult) GetPenaltiesV2() PenaltySettings`

GetPenaltiesV2 returns the PenaltiesV2 field if non-nil, zero value otherwise.

### GetPenaltiesV2Ok

`func (o *AssignmentSettingsResult) GetPenaltiesV2Ok() (*PenaltySettings, bool)`

GetPenaltiesV2Ok returns a tuple with the PenaltiesV2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPenaltiesV2

`func (o *AssignmentSettingsResult) SetPenaltiesV2(v PenaltySettings)`

SetPenaltiesV2 sets PenaltiesV2 field to given value.

### HasPenaltiesV2

`func (o *AssignmentSettingsResult) HasPenaltiesV2() bool`

HasPenaltiesV2 returns a boolean if a field has been set.

### GetStartTime

`func (o *AssignmentSettingsResult) GetStartTime() string`

GetStartTime returns the StartTime field if non-nil, zero value otherwise.

### GetStartTimeOk

`func (o *AssignmentSettingsResult) GetStartTimeOk() (*string, bool)`

GetStartTimeOk returns a tuple with the StartTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStartTime

`func (o *AssignmentSettingsResult) SetStartTime(v string)`

SetStartTime sets StartTime field to given value.

### HasStartTime

`func (o *AssignmentSettingsResult) HasStartTime() bool`

HasStartTime returns a boolean if a field has been set.

### GetDueTime

`func (o *AssignmentSettingsResult) GetDueTime() string`

GetDueTime returns the DueTime field if non-nil, zero value otherwise.

### GetDueTimeOk

`func (o *AssignmentSettingsResult) GetDueTimeOk() (*string, bool)`

GetDueTimeOk returns a tuple with the DueTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDueTime

`func (o *AssignmentSettingsResult) SetDueTime(v string)`

SetDueTime sets DueTime field to given value.

### HasDueTime

`func (o *AssignmentSettingsResult) HasDueTime() bool`

HasDueTime returns a boolean if a field has been set.

### GetMarkAsCompleteOnDueDate

`func (o *AssignmentSettingsResult) GetMarkAsCompleteOnDueDate() bool`

GetMarkAsCompleteOnDueDate returns the MarkAsCompleteOnDueDate field if non-nil, zero value otherwise.

### GetMarkAsCompleteOnDueDateOk

`func (o *AssignmentSettingsResult) GetMarkAsCompleteOnDueDateOk() (*bool, bool)`

GetMarkAsCompleteOnDueDateOk returns a tuple with the MarkAsCompleteOnDueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarkAsCompleteOnDueDate

`func (o *AssignmentSettingsResult) SetMarkAsCompleteOnDueDate(v bool)`

SetMarkAsCompleteOnDueDate sets MarkAsCompleteOnDueDate field to given value.

### HasMarkAsCompleteOnDueDate

`func (o *AssignmentSettingsResult) HasMarkAsCompleteOnDueDate() bool`

HasMarkAsCompleteOnDueDate returns a boolean if a field has been set.

### GetEndTime

`func (o *AssignmentSettingsResult) GetEndTime() string`

GetEndTime returns the EndTime field if non-nil, zero value otherwise.

### GetEndTimeOk

`func (o *AssignmentSettingsResult) GetEndTimeOk() (*string, bool)`

GetEndTimeOk returns a tuple with the EndTime field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEndTime

`func (o *AssignmentSettingsResult) SetEndTime(v string)`

SetEndTime sets EndTime field to given value.

### HasEndTime

`func (o *AssignmentSettingsResult) HasEndTime() bool`

HasEndTime returns a boolean if a field has been set.

### GetAction

`func (o *AssignmentSettingsResult) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *AssignmentSettingsResult) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *AssignmentSettingsResult) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *AssignmentSettingsResult) HasAction() bool`

HasAction returns a boolean if a field has been set.

### GetExamMode

`func (o *AssignmentSettingsResult) GetExamMode() ExamMode`

GetExamMode returns the ExamMode field if non-nil, zero value otherwise.

### GetExamModeOk

`func (o *AssignmentSettingsResult) GetExamModeOk() (*ExamMode, bool)`

GetExamModeOk returns a tuple with the ExamMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExamMode

`func (o *AssignmentSettingsResult) SetExamMode(v ExamMode)`

SetExamMode sets ExamMode field to given value.

### HasExamMode

`func (o *AssignmentSettingsResult) HasExamMode() bool`

HasExamMode returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



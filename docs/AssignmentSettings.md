# AssignmentSettings

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
**ExamMode** | Pointer to [**ExamMode**](ExamMode.md) |  | [optional] 
**Start** | Pointer to **string** |  | [optional] 
**Due** | Pointer to **string** |  | [optional] 
**MarkAsCompleteOnDueDate** | Pointer to **bool** |  | [optional] 
**End** | Pointer to **string** |  | [optional] 
**Action** | Pointer to **string** | Assignment action on completed | [optional] 

## Methods

### NewAssignmentSettings

`func NewAssignmentSettings() *AssignmentSettings`

NewAssignmentSettings instantiates a new AssignmentSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAssignmentSettingsWithDefaults

`func NewAssignmentSettingsWithDefaults() *AssignmentSettings`

NewAssignmentSettingsWithDefaults instantiates a new AssignmentSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetIsDisabled

`func (o *AssignmentSettings) GetIsDisabled() bool`

GetIsDisabled returns the IsDisabled field if non-nil, zero value otherwise.

### GetIsDisabledOk

`func (o *AssignmentSettings) GetIsDisabledOk() (*bool, bool)`

GetIsDisabledOk returns a tuple with the IsDisabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetIsDisabled

`func (o *AssignmentSettings) SetIsDisabled(v bool)`

SetIsDisabled sets IsDisabled field to given value.

### HasIsDisabled

`func (o *AssignmentSettings) HasIsDisabled() bool`

HasIsDisabled returns a boolean if a field has been set.

### GetReleaseGrades

`func (o *AssignmentSettings) GetReleaseGrades() bool`

GetReleaseGrades returns the ReleaseGrades field if non-nil, zero value otherwise.

### GetReleaseGradesOk

`func (o *AssignmentSettings) GetReleaseGradesOk() (*bool, bool)`

GetReleaseGradesOk returns a tuple with the ReleaseGrades field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReleaseGrades

`func (o *AssignmentSettings) SetReleaseGrades(v bool)`

SetReleaseGrades sets ReleaseGrades field to given value.

### HasReleaseGrades

`func (o *AssignmentSettings) HasReleaseGrades() bool`

HasReleaseGrades returns a boolean if a field has been set.

### GetEnableResetAssignmentByStudent

`func (o *AssignmentSettings) GetEnableResetAssignmentByStudent() bool`

GetEnableResetAssignmentByStudent returns the EnableResetAssignmentByStudent field if non-nil, zero value otherwise.

### GetEnableResetAssignmentByStudentOk

`func (o *AssignmentSettings) GetEnableResetAssignmentByStudentOk() (*bool, bool)`

GetEnableResetAssignmentByStudentOk returns a tuple with the EnableResetAssignmentByStudent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnableResetAssignmentByStudent

`func (o *AssignmentSettings) SetEnableResetAssignmentByStudent(v bool)`

SetEnableResetAssignmentByStudent sets EnableResetAssignmentByStudent field to given value.

### HasEnableResetAssignmentByStudent

`func (o *AssignmentSettings) HasEnableResetAssignmentByStudent() bool`

HasEnableResetAssignmentByStudent returns a boolean if a field has been set.

### GetDisableDownloadByStudent

`func (o *AssignmentSettings) GetDisableDownloadByStudent() bool`

GetDisableDownloadByStudent returns the DisableDownloadByStudent field if non-nil, zero value otherwise.

### GetDisableDownloadByStudentOk

`func (o *AssignmentSettings) GetDisableDownloadByStudentOk() (*bool, bool)`

GetDisableDownloadByStudentOk returns a tuple with the DisableDownloadByStudent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDisableDownloadByStudent

`func (o *AssignmentSettings) SetDisableDownloadByStudent(v bool)`

SetDisableDownloadByStudent sets DisableDownloadByStudent field to given value.

### HasDisableDownloadByStudent

`func (o *AssignmentSettings) HasDisableDownloadByStudent() bool`

HasDisableDownloadByStudent returns a boolean if a field has been set.

### GetVisibilityOnDisabled

`func (o *AssignmentSettings) GetVisibilityOnDisabled() string`

GetVisibilityOnDisabled returns the VisibilityOnDisabled field if non-nil, zero value otherwise.

### GetVisibilityOnDisabledOk

`func (o *AssignmentSettings) GetVisibilityOnDisabledOk() (*string, bool)`

GetVisibilityOnDisabledOk returns a tuple with the VisibilityOnDisabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibilityOnDisabled

`func (o *AssignmentSettings) SetVisibilityOnDisabled(v string)`

SetVisibilityOnDisabled sets VisibilityOnDisabled field to given value.

### HasVisibilityOnDisabled

`func (o *AssignmentSettings) HasVisibilityOnDisabled() bool`

HasVisibilityOnDisabled returns a boolean if a field has been set.

### GetVisibilityOnCompleted

`func (o *AssignmentSettings) GetVisibilityOnCompleted() string`

GetVisibilityOnCompleted returns the VisibilityOnCompleted field if non-nil, zero value otherwise.

### GetVisibilityOnCompletedOk

`func (o *AssignmentSettings) GetVisibilityOnCompletedOk() (*string, bool)`

GetVisibilityOnCompletedOk returns a tuple with the VisibilityOnCompleted field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVisibilityOnCompleted

`func (o *AssignmentSettings) SetVisibilityOnCompleted(v string)`

SetVisibilityOnCompleted sets VisibilityOnCompleted field to given value.

### HasVisibilityOnCompleted

`func (o *AssignmentSettings) HasVisibilityOnCompleted() bool`

HasVisibilityOnCompleted returns a boolean if a field has been set.

### GetPenaltiesV2

`func (o *AssignmentSettings) GetPenaltiesV2() PenaltySettings`

GetPenaltiesV2 returns the PenaltiesV2 field if non-nil, zero value otherwise.

### GetPenaltiesV2Ok

`func (o *AssignmentSettings) GetPenaltiesV2Ok() (*PenaltySettings, bool)`

GetPenaltiesV2Ok returns a tuple with the PenaltiesV2 field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPenaltiesV2

`func (o *AssignmentSettings) SetPenaltiesV2(v PenaltySettings)`

SetPenaltiesV2 sets PenaltiesV2 field to given value.

### HasPenaltiesV2

`func (o *AssignmentSettings) HasPenaltiesV2() bool`

HasPenaltiesV2 returns a boolean if a field has been set.

### GetExamMode

`func (o *AssignmentSettings) GetExamMode() ExamMode`

GetExamMode returns the ExamMode field if non-nil, zero value otherwise.

### GetExamModeOk

`func (o *AssignmentSettings) GetExamModeOk() (*ExamMode, bool)`

GetExamModeOk returns a tuple with the ExamMode field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetExamMode

`func (o *AssignmentSettings) SetExamMode(v ExamMode)`

SetExamMode sets ExamMode field to given value.

### HasExamMode

`func (o *AssignmentSettings) HasExamMode() bool`

HasExamMode returns a boolean if a field has been set.

### GetStart

`func (o *AssignmentSettings) GetStart() string`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *AssignmentSettings) GetStartOk() (*string, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *AssignmentSettings) SetStart(v string)`

SetStart sets Start field to given value.

### HasStart

`func (o *AssignmentSettings) HasStart() bool`

HasStart returns a boolean if a field has been set.

### GetDue

`func (o *AssignmentSettings) GetDue() string`

GetDue returns the Due field if non-nil, zero value otherwise.

### GetDueOk

`func (o *AssignmentSettings) GetDueOk() (*string, bool)`

GetDueOk returns a tuple with the Due field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDue

`func (o *AssignmentSettings) SetDue(v string)`

SetDue sets Due field to given value.

### HasDue

`func (o *AssignmentSettings) HasDue() bool`

HasDue returns a boolean if a field has been set.

### GetMarkAsCompleteOnDueDate

`func (o *AssignmentSettings) GetMarkAsCompleteOnDueDate() bool`

GetMarkAsCompleteOnDueDate returns the MarkAsCompleteOnDueDate field if non-nil, zero value otherwise.

### GetMarkAsCompleteOnDueDateOk

`func (o *AssignmentSettings) GetMarkAsCompleteOnDueDateOk() (*bool, bool)`

GetMarkAsCompleteOnDueDateOk returns a tuple with the MarkAsCompleteOnDueDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetMarkAsCompleteOnDueDate

`func (o *AssignmentSettings) SetMarkAsCompleteOnDueDate(v bool)`

SetMarkAsCompleteOnDueDate sets MarkAsCompleteOnDueDate field to given value.

### HasMarkAsCompleteOnDueDate

`func (o *AssignmentSettings) HasMarkAsCompleteOnDueDate() bool`

HasMarkAsCompleteOnDueDate returns a boolean if a field has been set.

### GetEnd

`func (o *AssignmentSettings) GetEnd() string`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *AssignmentSettings) GetEndOk() (*string, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *AssignmentSettings) SetEnd(v string)`

SetEnd sets End field to given value.

### HasEnd

`func (o *AssignmentSettings) HasEnd() bool`

HasEnd returns a boolean if a field has been set.

### GetAction

`func (o *AssignmentSettings) GetAction() string`

GetAction returns the Action field if non-nil, zero value otherwise.

### GetActionOk

`func (o *AssignmentSettings) GetActionOk() (*string, bool)`

GetActionOk returns a tuple with the Action field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAction

`func (o *AssignmentSettings) SetAction(v string)`

SetAction sets Action field to given value.

### HasAction

`func (o *AssignmentSettings) HasAction() bool`

HasAction returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



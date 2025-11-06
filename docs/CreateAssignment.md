# CreateAssignment

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**ModuleId** | Pointer to **string** | Module identifier | [optional] 
**Settings** | Pointer to [**CreateAssignmentSettings**](CreateAssignmentSettings.md) | Settings for the assignment | [optional] 

## Methods

### NewCreateAssignment

`func NewCreateAssignment() *CreateAssignment`

NewCreateAssignment instantiates a new CreateAssignment object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAssignmentWithDefaults

`func NewCreateAssignmentWithDefaults() *CreateAssignment`

NewCreateAssignmentWithDefaults instantiates a new CreateAssignment object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetModuleId

`func (o *CreateAssignment) GetModuleId() string`

GetModuleId returns the ModuleId field if non-nil, zero value otherwise.

### GetModuleIdOk

`func (o *CreateAssignment) GetModuleIdOk() (*string, bool)`

GetModuleIdOk returns a tuple with the ModuleId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModuleId

`func (o *CreateAssignment) SetModuleId(v string)`

SetModuleId sets ModuleId field to given value.

### HasModuleId

`func (o *CreateAssignment) HasModuleId() bool`

HasModuleId returns a boolean if a field has been set.

### GetSettings

`func (o *CreateAssignment) GetSettings() CreateAssignmentSettings`

GetSettings returns the Settings field if non-nil, zero value otherwise.

### GetSettingsOk

`func (o *CreateAssignment) GetSettingsOk() (*CreateAssignmentSettings, bool)`

GetSettingsOk returns a tuple with the Settings field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetSettings

`func (o *CreateAssignment) SetSettings(v CreateAssignmentSettings)`

SetSettings sets Settings field to given value.

### HasSettings

`func (o *CreateAssignment) HasSettings() bool`

HasSettings returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



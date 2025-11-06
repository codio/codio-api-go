# CreateAssignmentSettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** | Name of the assignment | [optional] 
**Description** | Pointer to **string** | Description of the assignment | [optional] 
**GigaboxSlot** | Pointer to [**GigaBoxSlot**](GigaBoxSlot.md) | GigaBox slot for the assignment | [optional] 

## Methods

### NewCreateAssignmentSettings

`func NewCreateAssignmentSettings() *CreateAssignmentSettings`

NewCreateAssignmentSettings instantiates a new CreateAssignmentSettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateAssignmentSettingsWithDefaults

`func NewCreateAssignmentSettingsWithDefaults() *CreateAssignmentSettings`

NewCreateAssignmentSettingsWithDefaults instantiates a new CreateAssignmentSettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateAssignmentSettings) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateAssignmentSettings) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateAssignmentSettings) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CreateAssignmentSettings) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *CreateAssignmentSettings) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateAssignmentSettings) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateAssignmentSettings) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateAssignmentSettings) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetGigaboxSlot

`func (o *CreateAssignmentSettings) GetGigaboxSlot() GigaBoxSlot`

GetGigaboxSlot returns the GigaboxSlot field if non-nil, zero value otherwise.

### GetGigaboxSlotOk

`func (o *CreateAssignmentSettings) GetGigaboxSlotOk() (*GigaBoxSlot, bool)`

GetGigaboxSlotOk returns a tuple with the GigaboxSlot field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGigaboxSlot

`func (o *CreateAssignmentSettings) SetGigaboxSlot(v GigaBoxSlot)`

SetGigaboxSlot sets GigaboxSlot field to given value.

### HasGigaboxSlot

`func (o *CreateAssignmentSettings) HasGigaboxSlot() bool`

HasGigaboxSlot returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



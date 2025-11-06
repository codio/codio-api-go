# PenaltySettings

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Enabled** | Pointer to **bool** |  | [optional] 
**DeductionIntervalMinutes** | Pointer to **int32** |  | [optional] 
**DeductionPercent** | Pointer to **int32** |  | [optional] 
**LowestGradePercent** | Pointer to **int32** |  | [optional] 

## Methods

### NewPenaltySettings

`func NewPenaltySettings() *PenaltySettings`

NewPenaltySettings instantiates a new PenaltySettings object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewPenaltySettingsWithDefaults

`func NewPenaltySettingsWithDefaults() *PenaltySettings`

NewPenaltySettingsWithDefaults instantiates a new PenaltySettings object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetEnabled

`func (o *PenaltySettings) GetEnabled() bool`

GetEnabled returns the Enabled field if non-nil, zero value otherwise.

### GetEnabledOk

`func (o *PenaltySettings) GetEnabledOk() (*bool, bool)`

GetEnabledOk returns a tuple with the Enabled field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnabled

`func (o *PenaltySettings) SetEnabled(v bool)`

SetEnabled sets Enabled field to given value.

### HasEnabled

`func (o *PenaltySettings) HasEnabled() bool`

HasEnabled returns a boolean if a field has been set.

### GetDeductionIntervalMinutes

`func (o *PenaltySettings) GetDeductionIntervalMinutes() int32`

GetDeductionIntervalMinutes returns the DeductionIntervalMinutes field if non-nil, zero value otherwise.

### GetDeductionIntervalMinutesOk

`func (o *PenaltySettings) GetDeductionIntervalMinutesOk() (*int32, bool)`

GetDeductionIntervalMinutesOk returns a tuple with the DeductionIntervalMinutes field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeductionIntervalMinutes

`func (o *PenaltySettings) SetDeductionIntervalMinutes(v int32)`

SetDeductionIntervalMinutes sets DeductionIntervalMinutes field to given value.

### HasDeductionIntervalMinutes

`func (o *PenaltySettings) HasDeductionIntervalMinutes() bool`

HasDeductionIntervalMinutes returns a boolean if a field has been set.

### GetDeductionPercent

`func (o *PenaltySettings) GetDeductionPercent() int32`

GetDeductionPercent returns the DeductionPercent field if non-nil, zero value otherwise.

### GetDeductionPercentOk

`func (o *PenaltySettings) GetDeductionPercentOk() (*int32, bool)`

GetDeductionPercentOk returns a tuple with the DeductionPercent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDeductionPercent

`func (o *PenaltySettings) SetDeductionPercent(v int32)`

SetDeductionPercent sets DeductionPercent field to given value.

### HasDeductionPercent

`func (o *PenaltySettings) HasDeductionPercent() bool`

HasDeductionPercent returns a boolean if a field has been set.

### GetLowestGradePercent

`func (o *PenaltySettings) GetLowestGradePercent() int32`

GetLowestGradePercent returns the LowestGradePercent field if non-nil, zero value otherwise.

### GetLowestGradePercentOk

`func (o *PenaltySettings) GetLowestGradePercentOk() (*int32, bool)`

GetLowestGradePercentOk returns a tuple with the LowestGradePercent field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLowestGradePercent

`func (o *PenaltySettings) SetLowestGradePercent(v int32)`

SetLowestGradePercent sets LowestGradePercent field to given value.

### HasLowestGradePercent

`func (o *PenaltySettings) HasLowestGradePercent() bool`

HasLowestGradePercent returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# CreateCourse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** | Name of the course | [optional] 
**Description** | Pointer to **string** | Description of the course | [optional] 
**Start** | Pointer to **string** | Course start date and time, ISO Date String | [optional] 
**End** | Pointer to **string** | Course end date and time, ISO Date String | [optional] 
**Timezone** | Pointer to **string** | Timezone of the course | [optional] 
**Tags** | Pointer to **[]string** | Tags associated with the course | [optional] 

## Methods

### NewCreateCourse

`func NewCreateCourse() *CreateCourse`

NewCreateCourse instantiates a new CreateCourse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCreateCourseWithDefaults

`func NewCreateCourseWithDefaults() *CreateCourse`

NewCreateCourseWithDefaults instantiates a new CreateCourse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *CreateCourse) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *CreateCourse) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *CreateCourse) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *CreateCourse) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *CreateCourse) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *CreateCourse) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *CreateCourse) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *CreateCourse) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetStart

`func (o *CreateCourse) GetStart() string`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *CreateCourse) GetStartOk() (*string, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *CreateCourse) SetStart(v string)`

SetStart sets Start field to given value.

### HasStart

`func (o *CreateCourse) HasStart() bool`

HasStart returns a boolean if a field has been set.

### GetEnd

`func (o *CreateCourse) GetEnd() string`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *CreateCourse) GetEndOk() (*string, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *CreateCourse) SetEnd(v string)`

SetEnd sets End field to given value.

### HasEnd

`func (o *CreateCourse) HasEnd() bool`

HasEnd returns a boolean if a field has been set.

### GetTimezone

`func (o *CreateCourse) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *CreateCourse) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *CreateCourse) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *CreateCourse) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### GetTags

`func (o *CreateCourse) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *CreateCourse) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *CreateCourse) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *CreateCourse) HasTags() bool`

HasTags returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



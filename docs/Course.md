# Course

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Name** | Pointer to **string** | Course name | [optional] 
**Description** | Pointer to **string** | Course description | [optional] 
**Start** | Pointer to **string** | Course start date, ISO Date String | [optional] 
**End** | Pointer to **string** | Course end date, ISO Date String | [optional] 
**Timezone** | Pointer to **string** | Course timezone | [optional] 
**Tags** | Pointer to **[]string** | Course tags | [optional] 
**Id** | Pointer to **string** | Course identifier | [optional] 
**Modules** | Pointer to [**[]Module**](Module.md) |  | [optional] 
**CreationDate** | Pointer to **string** | Course create date, ISO Date String | [optional] 
**ArchivedDate** | Pointer to **string** | Course archive date, ISO Date String | [optional] 
**Archived** | Pointer to **bool** | Archived course state | [optional] 

## Methods

### NewCourse

`func NewCourse() *Course`

NewCourse instantiates a new Course object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewCourseWithDefaults

`func NewCourseWithDefaults() *Course`

NewCourseWithDefaults instantiates a new Course object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetName

`func (o *Course) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Course) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Course) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *Course) HasName() bool`

HasName returns a boolean if a field has been set.

### GetDescription

`func (o *Course) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Course) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Course) SetDescription(v string)`

SetDescription sets Description field to given value.

### HasDescription

`func (o *Course) HasDescription() bool`

HasDescription returns a boolean if a field has been set.

### GetStart

`func (o *Course) GetStart() string`

GetStart returns the Start field if non-nil, zero value otherwise.

### GetStartOk

`func (o *Course) GetStartOk() (*string, bool)`

GetStartOk returns a tuple with the Start field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStart

`func (o *Course) SetStart(v string)`

SetStart sets Start field to given value.

### HasStart

`func (o *Course) HasStart() bool`

HasStart returns a boolean if a field has been set.

### GetEnd

`func (o *Course) GetEnd() string`

GetEnd returns the End field if non-nil, zero value otherwise.

### GetEndOk

`func (o *Course) GetEndOk() (*string, bool)`

GetEndOk returns a tuple with the End field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetEnd

`func (o *Course) SetEnd(v string)`

SetEnd sets End field to given value.

### HasEnd

`func (o *Course) HasEnd() bool`

HasEnd returns a boolean if a field has been set.

### GetTimezone

`func (o *Course) GetTimezone() string`

GetTimezone returns the Timezone field if non-nil, zero value otherwise.

### GetTimezoneOk

`func (o *Course) GetTimezoneOk() (*string, bool)`

GetTimezoneOk returns a tuple with the Timezone field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTimezone

`func (o *Course) SetTimezone(v string)`

SetTimezone sets Timezone field to given value.

### HasTimezone

`func (o *Course) HasTimezone() bool`

HasTimezone returns a boolean if a field has been set.

### GetTags

`func (o *Course) GetTags() []string`

GetTags returns the Tags field if non-nil, zero value otherwise.

### GetTagsOk

`func (o *Course) GetTagsOk() (*[]string, bool)`

GetTagsOk returns a tuple with the Tags field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTags

`func (o *Course) SetTags(v []string)`

SetTags sets Tags field to given value.

### HasTags

`func (o *Course) HasTags() bool`

HasTags returns a boolean if a field has been set.

### GetId

`func (o *Course) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Course) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Course) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Course) HasId() bool`

HasId returns a boolean if a field has been set.

### GetModules

`func (o *Course) GetModules() []Module`

GetModules returns the Modules field if non-nil, zero value otherwise.

### GetModulesOk

`func (o *Course) GetModulesOk() (*[]Module, bool)`

GetModulesOk returns a tuple with the Modules field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetModules

`func (o *Course) SetModules(v []Module)`

SetModules sets Modules field to given value.

### HasModules

`func (o *Course) HasModules() bool`

HasModules returns a boolean if a field has been set.

### GetCreationDate

`func (o *Course) GetCreationDate() string`

GetCreationDate returns the CreationDate field if non-nil, zero value otherwise.

### GetCreationDateOk

`func (o *Course) GetCreationDateOk() (*string, bool)`

GetCreationDateOk returns a tuple with the CreationDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreationDate

`func (o *Course) SetCreationDate(v string)`

SetCreationDate sets CreationDate field to given value.

### HasCreationDate

`func (o *Course) HasCreationDate() bool`

HasCreationDate returns a boolean if a field has been set.

### GetArchivedDate

`func (o *Course) GetArchivedDate() string`

GetArchivedDate returns the ArchivedDate field if non-nil, zero value otherwise.

### GetArchivedDateOk

`func (o *Course) GetArchivedDateOk() (*string, bool)`

GetArchivedDateOk returns a tuple with the ArchivedDate field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchivedDate

`func (o *Course) SetArchivedDate(v string)`

SetArchivedDate sets ArchivedDate field to given value.

### HasArchivedDate

`func (o *Course) HasArchivedDate() bool`

HasArchivedDate returns a boolean if a field has been set.

### GetArchived

`func (o *Course) GetArchived() bool`

GetArchived returns the Archived field if non-nil, zero value otherwise.

### GetArchivedOk

`func (o *Course) GetArchivedOk() (*bool, bool)`

GetArchivedOk returns a tuple with the Archived field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetArchived

`func (o *Course) SetArchived(v bool)`

SetArchived sets Archived field to given value.

### HasArchived

`func (o *Course) HasArchived() bool`

HasArchived returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



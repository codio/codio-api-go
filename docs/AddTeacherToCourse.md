# AddTeacherToCourse

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**UserId** | Pointer to **string** | User identifier | [optional] 
**ReadOnly** | Pointer to **bool** | Teacher access, it will be ignored for org owners. | [optional] 

## Methods

### NewAddTeacherToCourse

`func NewAddTeacherToCourse() *AddTeacherToCourse`

NewAddTeacherToCourse instantiates a new AddTeacherToCourse object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAddTeacherToCourseWithDefaults

`func NewAddTeacherToCourseWithDefaults() *AddTeacherToCourse`

NewAddTeacherToCourseWithDefaults instantiates a new AddTeacherToCourse object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetUserId

`func (o *AddTeacherToCourse) GetUserId() string`

GetUserId returns the UserId field if non-nil, zero value otherwise.

### GetUserIdOk

`func (o *AddTeacherToCourse) GetUserIdOk() (*string, bool)`

GetUserIdOk returns a tuple with the UserId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUserId

`func (o *AddTeacherToCourse) SetUserId(v string)`

SetUserId sets UserId field to given value.

### HasUserId

`func (o *AddTeacherToCourse) HasUserId() bool`

HasUserId returns a boolean if a field has been set.

### GetReadOnly

`func (o *AddTeacherToCourse) GetReadOnly() bool`

GetReadOnly returns the ReadOnly field if non-nil, zero value otherwise.

### GetReadOnlyOk

`func (o *AddTeacherToCourse) GetReadOnlyOk() (*bool, bool)`

GetReadOnlyOk returns a tuple with the ReadOnly field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReadOnly

`func (o *AddTeacherToCourse) SetReadOnly(v bool)`

SetReadOnly sets ReadOnly field to given value.

### HasReadOnly

`func (o *AddTeacherToCourse) HasReadOnly() bool`

HasReadOnly returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



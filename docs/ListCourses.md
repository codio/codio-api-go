# ListCourses

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Courses** | Pointer to [**[]Course**](Course.md) | List of courses | [optional] 
**NextToken** | Pointer to **string** | If specified and not empty - next search data portion token | [optional] 

## Methods

### NewListCourses

`func NewListCourses() *ListCourses`

NewListCourses instantiates a new ListCourses object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewListCoursesWithDefaults

`func NewListCoursesWithDefaults() *ListCourses`

NewListCoursesWithDefaults instantiates a new ListCourses object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetCourses

`func (o *ListCourses) GetCourses() []Course`

GetCourses returns the Courses field if non-nil, zero value otherwise.

### GetCoursesOk

`func (o *ListCourses) GetCoursesOk() (*[]Course, bool)`

GetCoursesOk returns a tuple with the Courses field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCourses

`func (o *ListCourses) SetCourses(v []Course)`

SetCourses sets Courses field to given value.

### HasCourses

`func (o *ListCourses) HasCourses() bool`

HasCourses returns a boolean if a field has been set.

### GetNextToken

`func (o *ListCourses) GetNextToken() string`

GetNextToken returns the NextToken field if non-nil, zero value otherwise.

### GetNextTokenOk

`func (o *ListCourses) GetNextTokenOk() (*string, bool)`

GetNextTokenOk returns a tuple with the NextToken field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNextToken

`func (o *ListCourses) SetNextToken(v string)`

SetNextToken sets NextToken field to given value.

### HasNextToken

`func (o *ListCourses) HasNextToken() bool`

HasNextToken returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# AssignmentProgressItem

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**AssignmentName** | Pointer to **string** | Assignment name | [optional] 
**AssignmentId** | Pointer to **string** | Module id | [optional] 
**Started** | Pointer to **bool** |  | [optional] 
**Progress** | Pointer to [**AssignmentProgress**](AssignmentProgress.md) | Assignment progress | [optional] 

## Methods

### NewAssignmentProgressItem

`func NewAssignmentProgressItem() *AssignmentProgressItem`

NewAssignmentProgressItem instantiates a new AssignmentProgressItem object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewAssignmentProgressItemWithDefaults

`func NewAssignmentProgressItemWithDefaults() *AssignmentProgressItem`

NewAssignmentProgressItemWithDefaults instantiates a new AssignmentProgressItem object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetAssignmentName

`func (o *AssignmentProgressItem) GetAssignmentName() string`

GetAssignmentName returns the AssignmentName field if non-nil, zero value otherwise.

### GetAssignmentNameOk

`func (o *AssignmentProgressItem) GetAssignmentNameOk() (*string, bool)`

GetAssignmentNameOk returns a tuple with the AssignmentName field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignmentName

`func (o *AssignmentProgressItem) SetAssignmentName(v string)`

SetAssignmentName sets AssignmentName field to given value.

### HasAssignmentName

`func (o *AssignmentProgressItem) HasAssignmentName() bool`

HasAssignmentName returns a boolean if a field has been set.

### GetAssignmentId

`func (o *AssignmentProgressItem) GetAssignmentId() string`

GetAssignmentId returns the AssignmentId field if non-nil, zero value otherwise.

### GetAssignmentIdOk

`func (o *AssignmentProgressItem) GetAssignmentIdOk() (*string, bool)`

GetAssignmentIdOk returns a tuple with the AssignmentId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetAssignmentId

`func (o *AssignmentProgressItem) SetAssignmentId(v string)`

SetAssignmentId sets AssignmentId field to given value.

### HasAssignmentId

`func (o *AssignmentProgressItem) HasAssignmentId() bool`

HasAssignmentId returns a boolean if a field has been set.

### GetStarted

`func (o *AssignmentProgressItem) GetStarted() bool`

GetStarted returns the Started field if non-nil, zero value otherwise.

### GetStartedOk

`func (o *AssignmentProgressItem) GetStartedOk() (*bool, bool)`

GetStartedOk returns a tuple with the Started field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStarted

`func (o *AssignmentProgressItem) SetStarted(v bool)`

SetStarted sets Started field to given value.

### HasStarted

`func (o *AssignmentProgressItem) HasStarted() bool`

HasStarted returns a boolean if a field has been set.

### GetProgress

`func (o *AssignmentProgressItem) GetProgress() AssignmentProgress`

GetProgress returns the Progress field if non-nil, zero value otherwise.

### GetProgressOk

`func (o *AssignmentProgressItem) GetProgressOk() (*AssignmentProgress, bool)`

GetProgressOk returns a tuple with the Progress field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetProgress

`func (o *AssignmentProgressItem) SetProgress(v AssignmentProgress)`

SetProgress sets Progress field to given value.

### HasProgress

`func (o *AssignmentProgressItem) HasProgress() bool`

HasProgress returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# StackInfo

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**Name** | Pointer to **string** |  | [optional] 
**LongDescription** | Pointer to **string** |  | [optional] 
**ShortDescription** | Pointer to **string** |  | [optional] 
**Owner** | Pointer to **string** |  | [optional] 
**OwnerType** | Pointer to **string** |  | [optional] 
**Versions** | Pointer to [**[]StackVersionInfo**](StackVersionInfo.md) |  | [optional] 
**Installations** | Pointer to **int64** |  | [optional] 

## Methods

### NewStackInfo

`func NewStackInfo() *StackInfo`

NewStackInfo instantiates a new StackInfo object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewStackInfoWithDefaults

`func NewStackInfoWithDefaults() *StackInfo`

NewStackInfoWithDefaults instantiates a new StackInfo object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *StackInfo) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *StackInfo) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *StackInfo) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *StackInfo) HasId() bool`

HasId returns a boolean if a field has been set.

### GetName

`func (o *StackInfo) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *StackInfo) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *StackInfo) SetName(v string)`

SetName sets Name field to given value.

### HasName

`func (o *StackInfo) HasName() bool`

HasName returns a boolean if a field has been set.

### GetLongDescription

`func (o *StackInfo) GetLongDescription() string`

GetLongDescription returns the LongDescription field if non-nil, zero value otherwise.

### GetLongDescriptionOk

`func (o *StackInfo) GetLongDescriptionOk() (*string, bool)`

GetLongDescriptionOk returns a tuple with the LongDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetLongDescription

`func (o *StackInfo) SetLongDescription(v string)`

SetLongDescription sets LongDescription field to given value.

### HasLongDescription

`func (o *StackInfo) HasLongDescription() bool`

HasLongDescription returns a boolean if a field has been set.

### GetShortDescription

`func (o *StackInfo) GetShortDescription() string`

GetShortDescription returns the ShortDescription field if non-nil, zero value otherwise.

### GetShortDescriptionOk

`func (o *StackInfo) GetShortDescriptionOk() (*string, bool)`

GetShortDescriptionOk returns a tuple with the ShortDescription field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetShortDescription

`func (o *StackInfo) SetShortDescription(v string)`

SetShortDescription sets ShortDescription field to given value.

### HasShortDescription

`func (o *StackInfo) HasShortDescription() bool`

HasShortDescription returns a boolean if a field has been set.

### GetOwner

`func (o *StackInfo) GetOwner() string`

GetOwner returns the Owner field if non-nil, zero value otherwise.

### GetOwnerOk

`func (o *StackInfo) GetOwnerOk() (*string, bool)`

GetOwnerOk returns a tuple with the Owner field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwner

`func (o *StackInfo) SetOwner(v string)`

SetOwner sets Owner field to given value.

### HasOwner

`func (o *StackInfo) HasOwner() bool`

HasOwner returns a boolean if a field has been set.

### GetOwnerType

`func (o *StackInfo) GetOwnerType() string`

GetOwnerType returns the OwnerType field if non-nil, zero value otherwise.

### GetOwnerTypeOk

`func (o *StackInfo) GetOwnerTypeOk() (*string, bool)`

GetOwnerTypeOk returns a tuple with the OwnerType field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOwnerType

`func (o *StackInfo) SetOwnerType(v string)`

SetOwnerType sets OwnerType field to given value.

### HasOwnerType

`func (o *StackInfo) HasOwnerType() bool`

HasOwnerType returns a boolean if a field has been set.

### GetVersions

`func (o *StackInfo) GetVersions() []StackVersionInfo`

GetVersions returns the Versions field if non-nil, zero value otherwise.

### GetVersionsOk

`func (o *StackInfo) GetVersionsOk() (*[]StackVersionInfo, bool)`

GetVersionsOk returns a tuple with the Versions field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetVersions

`func (o *StackInfo) SetVersions(v []StackVersionInfo)`

SetVersions sets Versions field to given value.

### HasVersions

`func (o *StackInfo) HasVersions() bool`

HasVersions returns a boolean if a field has been set.

### GetInstallations

`func (o *StackInfo) GetInstallations() int64`

GetInstallations returns the Installations field if non-nil, zero value otherwise.

### GetInstallationsOk

`func (o *StackInfo) GetInstallationsOk() (*int64, bool)`

GetInstallationsOk returns a tuple with the Installations field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInstallations

`func (o *StackInfo) SetInstallations(v int64)`

SetInstallations sets Installations field to given value.

### HasInstallations

`func (o *StackInfo) HasInstallations() bool`

HasInstallations returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



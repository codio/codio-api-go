# DownloadStatus

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**TaskId** | Pointer to **string** | Task identification | [optional] 
**Done** | Pointer to **bool** | Task status | [optional] 
**Url** | Pointer to **string** | If task completed - url for download | [optional] 
**Error** | Pointer to **string** | Error description if task failed | [optional] 

## Methods

### NewDownloadStatus

`func NewDownloadStatus() *DownloadStatus`

NewDownloadStatus instantiates a new DownloadStatus object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewDownloadStatusWithDefaults

`func NewDownloadStatusWithDefaults() *DownloadStatus`

NewDownloadStatusWithDefaults instantiates a new DownloadStatus object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTaskId

`func (o *DownloadStatus) GetTaskId() string`

GetTaskId returns the TaskId field if non-nil, zero value otherwise.

### GetTaskIdOk

`func (o *DownloadStatus) GetTaskIdOk() (*string, bool)`

GetTaskIdOk returns a tuple with the TaskId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTaskId

`func (o *DownloadStatus) SetTaskId(v string)`

SetTaskId sets TaskId field to given value.

### HasTaskId

`func (o *DownloadStatus) HasTaskId() bool`

HasTaskId returns a boolean if a field has been set.

### GetDone

`func (o *DownloadStatus) GetDone() bool`

GetDone returns the Done field if non-nil, zero value otherwise.

### GetDoneOk

`func (o *DownloadStatus) GetDoneOk() (*bool, bool)`

GetDoneOk returns a tuple with the Done field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDone

`func (o *DownloadStatus) SetDone(v bool)`

SetDone sets Done field to given value.

### HasDone

`func (o *DownloadStatus) HasDone() bool`

HasDone returns a boolean if a field has been set.

### GetUrl

`func (o *DownloadStatus) GetUrl() string`

GetUrl returns the Url field if non-nil, zero value otherwise.

### GetUrlOk

`func (o *DownloadStatus) GetUrlOk() (*string, bool)`

GetUrlOk returns a tuple with the Url field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetUrl

`func (o *DownloadStatus) SetUrl(v string)`

SetUrl sets Url field to given value.

### HasUrl

`func (o *DownloadStatus) HasUrl() bool`

HasUrl returns a boolean if a field has been set.

### GetError

`func (o *DownloadStatus) GetError() string`

GetError returns the Error field if non-nil, zero value otherwise.

### GetErrorOk

`func (o *DownloadStatus) GetErrorOk() (*string, bool)`

GetErrorOk returns a tuple with the Error field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetError

`func (o *DownloadStatus) SetError(v string)`

SetError sets Error field to given value.

### HasError

`func (o *DownloadStatus) HasError() bool`

HasError returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# \StackAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**StackInfo**](StackAPIAPI.md#StackInfo) | **Get** /api/v1/stacks/{stackId} | Get stack information
[**StackVersionsPublish**](StackAPIAPI.md#StackVersionsPublish) | **Post** /api/v1/stacks/{stackId}/versions | Publish new stack version
[**StackVersionsPublishStatus**](StackAPIAPI.md#StackVersionsPublishStatus) | **Get** /api/v1/stacks/{stackId}/tasks/{taskId} | Get stack version publish information



## StackInfo

> StackInfo StackInfo(ctx, stackId).Execute()

Get stack information

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/codio/codio-api-go"
)

func main() {
	stackId := "stackId_example" // string | Stack id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StackAPIAPI.StackInfo(context.Background(), stackId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StackAPIAPI.StackInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StackInfo`: StackInfo
	fmt.Fprintf(os.Stdout, "Response from `StackAPIAPI.StackInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**stackId** | **string** | Stack id |

### Other Parameters

Other parameters are passed through a pointer to a apiStackInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**StackInfo**](StackInfo.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StackVersionsPublish

> TaskProgress StackVersionsPublish(ctx, stackId).Id(id).Provisioner(provisioner).Content(content).Message(message).File(file).Execute()

Publish new stack version

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/codio/codio-api-go"
)

func main() {
	stackId := "stackId_example" // string | Stack id
	id := "id_example" // string |
	provisioner := "provisioner_example" // string | Provisioner type (optional)
	content := "content_example" // string | Optional provision instructions. Content or bundle should be specified (optional)
	message := "message_example" // string |  (optional)
	file := os.NewFile(1234, "some_file") // *os.File | Optional bundle for provisioner. Content or bundle should be specified (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StackAPIAPI.StackVersionsPublish(context.Background(), stackId).Id(id).Provisioner(provisioner).Content(content).Message(message).File(file).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StackAPIAPI.StackVersionsPublish``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StackVersionsPublish`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `StackAPIAPI.StackVersionsPublish`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**stackId** | **string** | Stack id |

### Other Parameters

Other parameters are passed through a pointer to a apiStackVersionsPublishRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **id** | **string** |  |
 **provisioner** | **string** | Provisioner type |
 **content** | **string** | Optional provision instructions. Content or bundle should be specified |
 **message** | **string** |  |
 **file** | ***os.File** | Optional bundle for provisioner. Content or bundle should be specified |

### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StackVersionsPublishStatus

> StackPublishInfo StackVersionsPublishStatus(ctx, stackId, taskId).Execute()

Get stack version publish information

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/codio/codio-api-go"
)

func main() {
	stackId := "stackId_example" // string | Stack id
	taskId := "taskId_example" // string | Task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.StackAPIAPI.StackVersionsPublishStatus(context.Background(), stackId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `StackAPIAPI.StackVersionsPublishStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StackVersionsPublishStatus`: StackPublishInfo
	fmt.Fprintf(os.Stdout, "Response from `StackAPIAPI.StackVersionsPublishStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**stackId** | **string** | Stack id |
**taskId** | **string** | Task id |

### Other Parameters

Other parameters are passed through a pointer to a apiStackVersionsPublishStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**StackPublishInfo**](StackPublishInfo.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

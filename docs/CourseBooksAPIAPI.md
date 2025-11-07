# \CourseBooksAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**BookVersionPublish**](CourseBooksAPIAPI.md#BookVersionPublish) | **Post** /api/v1/books/{bookId}/versions | Publish new book version
[**BookVersionPublishesStatus**](CourseBooksAPIAPI.md#BookVersionPublishesStatus) | **Get** /api/v1/books/{bookId}/publishes/{taskId} | Get book publish status



## BookVersionPublish

> TaskProgress BookVersionPublish(ctx, bookId).File(file).Changelog(changelog).StackVersionId(stackVersionId).WithStackUpdate(withStackUpdate).Execute()

Publish new book version

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
	bookId := "bookId_example" // string | Book id
	file := os.NewFile(1234, "some_file") // *os.File | File archive data to be published (optional)
	changelog := "changelog_example" // string | Publish changelog (optional)
	stackVersionId := "stackVersionId_example" // string | Stack version identification (optional)
	withStackUpdate := true // bool | Propagate stack update (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseBooksAPIAPI.BookVersionPublish(context.Background(), bookId).File(file).Changelog(changelog).StackVersionId(stackVersionId).WithStackUpdate(withStackUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseBooksAPIAPI.BookVersionPublish``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookVersionPublish`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseBooksAPIAPI.BookVersionPublish`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bookId** | **string** | Book id |

### Other Parameters

Other parameters are passed through a pointer to a apiBookVersionPublishRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **file** | ***os.File** | File archive data to be published |
 **changelog** | **string** | Publish changelog |
 **stackVersionId** | **string** | Stack version identification |
 **withStackUpdate** | **bool** | Propagate stack update |

### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## BookVersionPublishesStatus

> TaskStatus BookVersionPublishesStatus(ctx, bookId, taskId).Execute()

Get book publish status

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
	bookId := "bookId_example" // string | Book id
	taskId := "taskId_example" // string | Task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseBooksAPIAPI.BookVersionPublishesStatus(context.Background(), bookId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseBooksAPIAPI.BookVersionPublishesStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `BookVersionPublishesStatus`: TaskStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseBooksAPIAPI.BookVersionPublishesStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**bookId** | **string** | Book id |
**taskId** | **string** | Task id |

### Other Parameters

Other parameters are passed through a pointer to a apiBookVersionPublishesStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**TaskStatus**](TaskStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

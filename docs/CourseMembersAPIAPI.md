# \CourseMembersAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AddTeacher**](CourseMembersAPIAPI.md#AddTeacher) | **Post** /api/v1/courses/{courseId}/teachers | Add teacher to course



## AddTeacher

> AddTeacherToCourseAnswer AddTeacher(ctx, courseId).AddTeacherToCourse(addTeacherToCourse).Execute()

Add teacher to course

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
	courseId := "courseId_example" // string | Course id
	addTeacherToCourse := *openapiclient.NewAddTeacherToCourse() // AddTeacherToCourse |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseMembersAPIAPI.AddTeacher(context.Background(), courseId).AddTeacherToCourse(addTeacherToCourse).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseMembersAPIAPI.AddTeacher``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AddTeacher`: AddTeacherToCourseAnswer
	fmt.Fprintf(os.Stdout, "Response from `CourseMembersAPIAPI.AddTeacher`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiAddTeacherRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **addTeacherToCourse** | [**AddTeacherToCourse**](AddTeacherToCourse.md) |  |

### Return type

[**AddTeacherToCourseAnswer**](AddTeacherToCourseAnswer.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

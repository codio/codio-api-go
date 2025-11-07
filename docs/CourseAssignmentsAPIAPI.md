# \CourseAssignmentsAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AssignmentStudentsInfo**](CourseAssignmentsAPIAPI.md#AssignmentStudentsInfo) | **Get** /api/v1/courses/{courseId}/assignments/{assignmentId}/students | Get assignment students info
[**AssignmentVersionPublish**](CourseAssignmentsAPIAPI.md#AssignmentVersionPublish) | **Post** /api/v1/courses/{courseId}/assignments/{assignmentId}/versions | Publish new assignment version
[**AssignmentVersionPublishesStatus**](CourseAssignmentsAPIAPI.md#AssignmentVersionPublishesStatus) | **Get** /api/v1/courses/{courseId}/assignments/{assignmentId}/publishes/{taskId} | Get assignment publish status
[**CreateProjectBasedAssignment**](CourseAssignmentsAPIAPI.md#CreateProjectBasedAssignment) | **Post** /api/v1/courses/{courseId}/assignments | Create Project Based Assignment
[**FetchAssignmentSettings**](CourseAssignmentsAPIAPI.md#FetchAssignmentSettings) | **Get** /api/v1/courses/{courseId}/assignments/{assignmentId}/settings | Fetch Assignment Settings
[**UpdateAssignmentSettings**](CourseAssignmentsAPIAPI.md#UpdateAssignmentSettings) | **Post** /api/v1/courses/{courseId}/assignments/{assignmentId}/settings | Update Assignment Settings
[**UpdateStudentTimeExtensions**](CourseAssignmentsAPIAPI.md#UpdateStudentTimeExtensions) | **Post** /api/v1/courses/{courseId}/assignments/{assignmentId}/students/{studentId} | Update Student Time Extensions



## AssignmentStudentsInfo

> []StudentInformation AssignmentStudentsInfo(ctx, courseId, assignmentId).Execute()

Get assignment students info

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	assignmentId := "assignmentId_example" // string | Assignment id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.AssignmentStudentsInfo(context.Background(), courseId, assignmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.AssignmentStudentsInfo``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssignmentStudentsInfo`: []StudentInformation
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.AssignmentStudentsInfo`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssignmentStudentsInfoRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**[]StudentInformation**](StudentInformation.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AssignmentVersionPublish

> TaskProgress AssignmentVersionPublish(ctx, courseId, assignmentId).File(file).Changelog(changelog).StackVersionId(stackVersionId).WithStackUpdate(withStackUpdate).Execute()

Publish new assignment version

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	assignmentId := "assignmentId_example" // string | Assignment id
	file := os.NewFile(1234, "some_file") // *os.File | File archive data to be published (optional)
	changelog := "changelog_example" // string | Publish changelog (optional)
	stackVersionId := "stackVersionId_example" // string | Stack version identification (optional)
	withStackUpdate := true // bool | Propagate stack update (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.AssignmentVersionPublish(context.Background(), courseId, assignmentId).File(file).Changelog(changelog).StackVersionId(stackVersionId).WithStackUpdate(withStackUpdate).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.AssignmentVersionPublish``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssignmentVersionPublish`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.AssignmentVersionPublish`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssignmentVersionPublishRequest struct via the builder pattern


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


## AssignmentVersionPublishesStatus

> TaskStatus AssignmentVersionPublishesStatus(ctx, courseId, assignmentId, taskId).Execute()

Get assignment publish status

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	assignmentId := "assignmentId_example" // string | Assignment id
	taskId := "taskId_example" // string | Task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.AssignmentVersionPublishesStatus(context.Background(), courseId, assignmentId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.AssignmentVersionPublishesStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssignmentVersionPublishesStatus`: TaskStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.AssignmentVersionPublishesStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 
**taskId** | **string** | Task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssignmentVersionPublishesStatusRequest struct via the builder pattern


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


## CreateProjectBasedAssignment

> CreateAssignmentAnswer CreateProjectBasedAssignment(ctx, courseId).CreateAssignment(createAssignment).Execute()

Create Project Based Assignment

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	createAssignment := *openapiclient.NewCreateAssignment() // CreateAssignment |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.CreateProjectBasedAssignment(context.Background(), courseId).CreateAssignment(createAssignment).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.CreateProjectBasedAssignment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateProjectBasedAssignment`: CreateAssignmentAnswer
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.CreateProjectBasedAssignment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiCreateProjectBasedAssignmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createAssignment** | [**CreateAssignment**](CreateAssignment.md) |  | 

### Return type

[**CreateAssignmentAnswer**](CreateAssignmentAnswer.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FetchAssignmentSettings

> AssignmentSettingsResult FetchAssignmentSettings(ctx, courseId, assignmentId).Execute()

Fetch Assignment Settings

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	assignmentId := "assignmentId_example" // string | Assignment id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.FetchAssignmentSettings(context.Background(), courseId, assignmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.FetchAssignmentSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FetchAssignmentSettings`: AssignmentSettingsResult
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.FetchAssignmentSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiFetchAssignmentSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**AssignmentSettingsResult**](AssignmentSettingsResult.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateAssignmentSettings

> AssignmentSettingsResult UpdateAssignmentSettings(ctx, courseId, assignmentId).AssignmentSettings(assignmentSettings).Execute()

Update Assignment Settings

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	assignmentId := "assignmentId_example" // string | Assignment id
	assignmentSettings := *openapiclient.NewAssignmentSettings() // AssignmentSettings |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.UpdateAssignmentSettings(context.Background(), courseId, assignmentId).AssignmentSettings(assignmentSettings).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.UpdateAssignmentSettings``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateAssignmentSettings`: AssignmentSettingsResult
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.UpdateAssignmentSettings`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateAssignmentSettingsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **assignmentSettings** | [**AssignmentSettings**](AssignmentSettings.md) |  | 

### Return type

[**AssignmentSettingsResult**](AssignmentSettingsResult.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateStudentTimeExtensions

> string UpdateStudentTimeExtensions(ctx, courseId, assignmentId, studentId).StudentTimeExtension(studentTimeExtension).Execute()

Update Student Time Extensions

### Example

```go
package main

import (
	"context"
	"fmt"
	"os"
	openapiclient "github.com/GIT_USER_ID/GIT_REPO_ID"
)

func main() {
	courseId := "courseId_example" // string | Course id
	assignmentId := "assignmentId_example" // string | Assignment id
	studentId := "studentId_example" // string | Student id
	studentTimeExtension := *openapiclient.NewStudentTimeExtension() // StudentTimeExtension |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAssignmentsAPIAPI.UpdateStudentTimeExtensions(context.Background(), courseId, assignmentId, studentId).StudentTimeExtension(studentTimeExtension).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAssignmentsAPIAPI.UpdateStudentTimeExtensions``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateStudentTimeExtensions`: string
	fmt.Fprintf(os.Stdout, "Response from `CourseAssignmentsAPIAPI.UpdateStudentTimeExtensions`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 
**studentId** | **string** | Student id | 

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateStudentTimeExtensionsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



 **studentTimeExtension** | [**StudentTimeExtension**](StudentTimeExtension.md) |  | 

### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


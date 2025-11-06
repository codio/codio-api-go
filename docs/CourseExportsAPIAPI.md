# \CourseExportsAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ExportAssessmentData**](CourseExportsAPIAPI.md#ExportAssessmentData) | **Get** /api/v1/courses/{courseId}/export/assessments/csv | Export Assessment Data CSV
[**ExportAssignmentCSV**](CourseExportsAPIAPI.md#ExportAssignmentCSV) | **Get** /api/v1/courses/{courseId}/assignments/{assignmentId}/export/csv | Export Assignment CSV
[**ExportCoachData**](CourseExportsAPIAPI.md#ExportCoachData) | **Post** /api/v1/courses/{courseId}/export/coach | Export Coach Data
[**ExportCoachDataByTask**](CourseExportsAPIAPI.md#ExportCoachDataByTask) | **Get** /api/v1/courses/{courseId}/export/coach/progress/{taskId} | Fetch Export Coach Data Status
[**ExportCourseSourceDataItemByTask**](CourseExportsAPIAPI.md#ExportCourseSourceDataItemByTask) | **Get** /api/v1/courses/{courseId}/export/sources/progress/{taskId} | Fetch Export Sources Status
[**ExportCourseSourceDataItems**](CourseExportsAPIAPI.md#ExportCourseSourceDataItems) | **Get** /api/v1/courses/{courseId}/export/sources | List Exports Course Sources Data
[**ExportCourseSourcesData**](CourseExportsAPIAPI.md#ExportCourseSourcesData) | **Post** /api/v1/courses/{courseId}/export/sources | Export Course Sources
[**ExportCourseWorkData**](CourseExportsAPIAPI.md#ExportCourseWorkData) | **Post** /api/v1/courses/{courseId}/export/workdata | Export Course Work Data
[**ExportCourseWorkDataItemByTask**](CourseExportsAPIAPI.md#ExportCourseWorkDataItemByTask) | **Get** /api/v1/courses/{courseId}/export/workdata/progress/{taskId} | Fetch Export Work Data Status
[**ExportCourseWorkDataItems**](CourseExportsAPIAPI.md#ExportCourseWorkDataItems) | **Get** /api/v1/courses/{courseId}/export/workdata | List Exports Course Work Data
[**ExportLLMProxyData**](CourseExportsAPIAPI.md#ExportLLMProxyData) | **Post** /api/v1/courses/{courseId}/export/llmproxy | Export LLMProxy Data
[**ExportLLMProxyDataByTaskRoute**](CourseExportsAPIAPI.md#ExportLLMProxyDataByTaskRoute) | **Get** /api/v1/courses/{courseId}/export/llmproxy/progress/{taskId} | Fetch Export LLMProxy Data Status
[**ExportStudentCSV**](CourseExportsAPIAPI.md#ExportStudentCSV) | **Get** /api/v1/courses/{courseId}/students/{studentId}/export/csv | Export Student CSV
[**FetchDownloadStatus**](CourseExportsAPIAPI.md#FetchDownloadStatus) | **Get** /api/v1/courses/{courseId}/export/assessments/csv/download/{taskId} | Fetch Export Assessment Data CSV Status
[**FetchDownloadStatusStudent**](CourseExportsAPIAPI.md#FetchDownloadStatusStudent) | **Get** /api/v1/courses/{courseId}/assignments/{assignmentId}/students/{studentId}/download/{taskId} | Fetch Export Student Data CSV Status
[**StartedAssignmentDownload**](CourseExportsAPIAPI.md#StartedAssignmentDownload) | **Get** /api/v1/courses/{courseId}/assignments/{assignmentId}/students/{studentId}/download | Fetch Export Assessment Data CSV Status



## ExportAssessmentData

> TaskProgress ExportAssessmentData(ctx, courseId).Execute()

Export Assessment Data CSV

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportAssessmentData(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportAssessmentData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportAssessmentData`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportAssessmentData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportAssessmentDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportAssignmentCSV

> string ExportAssignmentCSV(ctx, courseId, assignmentId).Execute()

Export Assignment CSV

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
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportAssignmentCSV(context.Background(), courseId, assignmentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportAssignmentCSV``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportAssignmentCSV`: string
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportAssignmentCSV`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportAssignmentCSVRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCoachData

> TaskProgress ExportCoachData(ctx, courseId).Execute()

Export Coach Data

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCoachData(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCoachData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCoachData`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCoachData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCoachDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCoachDataByTask

> DownloadStatus ExportCoachDataByTask(ctx, courseId, taskId).Execute()

Fetch Export Coach Data Status

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
	taskId := "taskId_example" // string | Export task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCoachDataByTask(context.Background(), courseId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCoachDataByTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCoachDataByTask`: DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCoachDataByTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**taskId** | **string** | Export task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCoachDataByTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCourseSourceDataItemByTask

> DownloadStatus ExportCourseSourceDataItemByTask(ctx, courseId, taskId).Execute()

Fetch Export Sources Status

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
	taskId := "taskId_example" // string | Export task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCourseSourceDataItemByTask(context.Background(), courseId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCourseSourceDataItemByTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCourseSourceDataItemByTask`: DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCourseSourceDataItemByTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**taskId** | **string** | Export task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCourseSourceDataItemByTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCourseSourceDataItems

> []DownloadStatus ExportCourseSourceDataItems(ctx, courseId).Execute()

List Exports Course Sources Data

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCourseSourceDataItems(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCourseSourceDataItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCourseSourceDataItems`: []DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCourseSourceDataItems`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCourseSourceDataItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCourseSourcesData

> TaskProgress ExportCourseSourcesData(ctx, courseId).Execute()

Export Course Sources

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCourseSourcesData(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCourseSourcesData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCourseSourcesData`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCourseSourcesData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCourseSourcesDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCourseWorkData

> TaskProgress ExportCourseWorkData(ctx, courseId).Execute()

Export Course Work Data

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCourseWorkData(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCourseWorkData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCourseWorkData`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCourseWorkData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCourseWorkDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCourseWorkDataItemByTask

> DownloadStatus ExportCourseWorkDataItemByTask(ctx, courseId, taskId).Execute()

Fetch Export Work Data Status

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
	taskId := "taskId_example" // string | Export task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCourseWorkDataItemByTask(context.Background(), courseId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCourseWorkDataItemByTask``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCourseWorkDataItemByTask`: DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCourseWorkDataItemByTask`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**taskId** | **string** | Export task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCourseWorkDataItemByTaskRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportCourseWorkDataItems

> []DownloadStatus ExportCourseWorkDataItems(ctx, courseId).Execute()

List Exports Course Work Data

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportCourseWorkDataItems(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportCourseWorkDataItems``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportCourseWorkDataItems`: []DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportCourseWorkDataItems`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportCourseWorkDataItemsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportLLMProxyData

> TaskProgress ExportLLMProxyData(ctx, courseId).Execute()

Export LLMProxy Data

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportLLMProxyData(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportLLMProxyData``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportLLMProxyData`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportLLMProxyData`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportLLMProxyDataRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportLLMProxyDataByTaskRoute

> DownloadStatus ExportLLMProxyDataByTaskRoute(ctx, courseId, taskId).Execute()

Fetch Export LLMProxy Data Status

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
	taskId := "taskId_example" // string | Export task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportLLMProxyDataByTaskRoute(context.Background(), courseId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportLLMProxyDataByTaskRoute``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportLLMProxyDataByTaskRoute`: DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportLLMProxyDataByTaskRoute`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**taskId** | **string** | Export task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportLLMProxyDataByTaskRouteRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ExportStudentCSV

> string ExportStudentCSV(ctx, courseId, studentId).Execute()

Export Student CSV

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
	studentId := "studentId_example" // string | Student id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.ExportStudentCSV(context.Background(), courseId, studentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.ExportStudentCSV``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ExportStudentCSV`: string
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.ExportStudentCSV`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**studentId** | **string** | Student id | 

### Other Parameters

Other parameters are passed through a pointer to a apiExportStudentCSVRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FetchDownloadStatus

> DownloadStatus FetchDownloadStatus(ctx, courseId, taskId).Execute()

Fetch Export Assessment Data CSV Status

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
	taskId := "taskId_example" // string | Export task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.FetchDownloadStatus(context.Background(), courseId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.FetchDownloadStatus``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FetchDownloadStatus`: DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.FetchDownloadStatus`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**taskId** | **string** | Export task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiFetchDownloadStatusRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FetchDownloadStatusStudent

> DownloadStatus FetchDownloadStatusStudent(ctx, courseId, assignmentId, studentId, taskId).Execute()

Fetch Export Student Data CSV Status

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
	taskId := "taskId_example" // string | Export task id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.FetchDownloadStatusStudent(context.Background(), courseId, assignmentId, studentId, taskId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.FetchDownloadStatusStudent``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FetchDownloadStatusStudent`: DownloadStatus
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.FetchDownloadStatusStudent`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id | 
**assignmentId** | **string** | Assignment id | 
**studentId** | **string** | Student id | 
**taskId** | **string** | Export task id | 

### Other Parameters

Other parameters are passed through a pointer to a apiFetchDownloadStatusStudentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------





### Return type

[**DownloadStatus**](DownloadStatus.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StartedAssignmentDownload

> TaskProgress StartedAssignmentDownload(ctx, courseId, assignmentId, studentId).Execute()

Fetch Export Assessment Data CSV Status

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseExportsAPIAPI.StartedAssignmentDownload(context.Background(), courseId, assignmentId, studentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseExportsAPIAPI.StartedAssignmentDownload``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StartedAssignmentDownload`: TaskProgress
	fmt.Fprintf(os.Stdout, "Response from `CourseExportsAPIAPI.StartedAssignmentDownload`: %v\n", resp)
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

Other parameters are passed through a pointer to a apiStartedAssignmentDownloadRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------




### Return type

[**TaskProgress**](TaskProgress.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


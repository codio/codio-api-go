# \CourseAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ArchiveCourse**](CourseAPIAPI.md#ArchiveCourse) | **Post** /api/v1/courses/{courseId}/archive | Archive Course
[**CourseStructure**](CourseAPIAPI.md#CourseStructure) | **Get** /api/v1/courses/{courseId} | Fetch Course Structure
[**CoursesList**](CourseAPIAPI.md#CoursesList) | **Get** /api/v1/courses_list | List Organization Courses
[**CreateCourse**](CourseAPIAPI.md#CreateCourse) | **Post** /api/v1/courses | Create Course
[**CreateCourseModule**](CourseAPIAPI.md#CreateCourseModule) | **Post** /api/v1/courses/{courseId}/modules | Create Course Module
[**FilterLearnersForMentors**](CourseAPIAPI.md#FilterLearnersForMentors) | **Post** /api/v1/courses/{courseId}/filterLearnersForMentors | Filter Learners For Mentors
[**FindCourse**](CourseAPIAPI.md#FindCourse) | **Get** /api/v1/courses | Find Course
[**ListCourseStudents**](CourseAPIAPI.md#ListCourseStudents) | **Get** /api/v1/courses/{courseId}/students | List Course Students
[**ListCourseTeachers**](CourseAPIAPI.md#ListCourseTeachers) | **Get** /api/v1/courses/{courseId}/teachers | List Course Teachers
[**StudentCourseProgress**](CourseAPIAPI.md#StudentCourseProgress) | **Get** /api/v1/courses/{courseId}/students/{studentId}/progress | Fetch Course Structure
[**UpdateBooks**](CourseAPIAPI.md#UpdateBooks) | **Post** /api/v1/courses/{courseId}/update_books | Update Course Books



## ArchiveCourse

> ArchiveCourse ArchiveCourse(ctx, courseId).Execute()

Archive Course

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
	courseId := "courseId_example" // string | Course id to archive

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.ArchiveCourse(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.ArchiveCourse``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ArchiveCourse`: ArchiveCourse
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.ArchiveCourse`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id to archive |

### Other Parameters

Other parameters are passed through a pointer to a apiArchiveCourseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**ArchiveCourse**](ArchiveCourse.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CourseStructure

> Course CourseStructure(ctx, courseId).WithHiddenAssignments(withHiddenAssignments).Execute()

Fetch Course Structure

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
	withHiddenAssignments := "withHiddenAssignments_example" // string | Fetch hidden assignments (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.CourseStructure(context.Background(), courseId).WithHiddenAssignments(withHiddenAssignments).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.CourseStructure``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CourseStructure`: Course
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.CourseStructure`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiCourseStructureRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **withHiddenAssignments** | **string** | Fetch hidden assignments |

### Return type

[**Course**](Course.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CoursesList

> ListCourses CoursesList(ctx).NextToken(nextToken).Archived(archived).Execute()

List Organization Courses

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
	nextToken := "nextToken_example" // string | Next search data portion token, if specified - other parameters will be ignored (optional)
	archived := "archived_example" // string | Archived courses filter (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.CoursesList(context.Background()).NextToken(nextToken).Archived(archived).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.CoursesList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CoursesList`: ListCourses
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.CoursesList`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCoursesListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nextToken** | **string** | Next search data portion token, if specified - other parameters will be ignored |
 **archived** | **string** | Archived courses filter |

### Return type

[**ListCourses**](ListCourses.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateCourse

> CreateCourseAnswer CreateCourse(ctx).CreateCourse(createCourse).Execute()

Create Course

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
	createCourse := *openapiclient.NewCreateCourse() // CreateCourse |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.CreateCourse(context.Background()).CreateCourse(createCourse).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.CreateCourse``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCourse`: CreateCourseAnswer
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.CreateCourse`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiCreateCourseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createCourse** | [**CreateCourse**](CreateCourse.md) |  |

### Return type

[**CreateCourseAnswer**](CreateCourseAnswer.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## CreateCourseModule

> CreateCourseModuleAnswer CreateCourseModule(ctx, courseId).CreateCourseModule(createCourseModule).Execute()

Create Course Module

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
	createCourseModule := *openapiclient.NewCreateCourseModule() // CreateCourseModule |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.CreateCourseModule(context.Background(), courseId).CreateCourseModule(createCourseModule).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.CreateCourseModule``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `CreateCourseModule`: CreateCourseModuleAnswer
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.CreateCourseModule`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiCreateCourseModuleRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **createCourseModule** | [**CreateCourseModule**](CreateCourseModule.md) |  |

### Return type

[**CreateCourseModuleAnswer**](CreateCourseModuleAnswer.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FilterLearnersForMentors

> FilterLearnersForMentorsAnswerExample FilterLearnersForMentors(ctx, courseId).Body(body).Execute()

Filter Learners For Mentors

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
	body := "body_example" // string |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.FilterLearnersForMentors(context.Background(), courseId).Body(body).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.FilterLearnersForMentors``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FilterLearnersForMentors`: FilterLearnersForMentorsAnswerExample
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.FilterLearnersForMentors`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiFilterLearnersForMentorsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **body** | **string** |  |

### Return type

[**FilterLearnersForMentorsAnswerExample**](FilterLearnersForMentorsAnswerExample.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## FindCourse

> Course FindCourse(ctx).Name(name).WithHiddenAssignments(withHiddenAssignments).Execute()

Find Course

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
	name := "name_example" // string | Course name
	withHiddenAssignments := "withHiddenAssignments_example" // string | Fetch hidden assignments (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.FindCourse(context.Background()).Name(name).WithHiddenAssignments(withHiddenAssignments).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.FindCourse``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `FindCourse`: Course
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.FindCourse`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiFindCourseRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **string** | Course name |
 **withHiddenAssignments** | **string** | Fetch hidden assignments |

### Return type

[**Course**](Course.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCourseStudents

> []User ListCourseStudents(ctx, courseId).Execute()

List Course Students

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.ListCourseStudents(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.ListCourseStudents``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCourseStudents`: []User
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.ListCourseStudents`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiListCourseStudentsRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]User**](User.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListCourseTeachers

> []User ListCourseTeachers(ctx, courseId).Execute()

List Course Teachers

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.ListCourseTeachers(context.Background(), courseId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.ListCourseTeachers``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListCourseTeachers`: []User
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.ListCourseTeachers`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiListCourseTeachersRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


### Return type

[**[]User**](User.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## StudentCourseProgress

> []AssignmentProgressItem StudentCourseProgress(ctx, courseId, studentId).Execute()

Fetch Course Structure

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
	studentId := "studentId_example" // string | Student id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.StudentCourseProgress(context.Background(), courseId, studentId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.StudentCourseProgress``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `StudentCourseProgress`: []AssignmentProgressItem
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.StudentCourseProgress`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |
**studentId** | **string** | Student id |

### Other Parameters

Other parameters are passed through a pointer to a apiStudentCourseProgressRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------



### Return type

[**[]AssignmentProgressItem**](AssignmentProgressItem.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## UpdateBooks

> Course UpdateBooks(ctx, courseId).BookId(bookId).Execute()

Update Course Books

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
	bookId := "bookId_example" // string | Book id to process (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.CourseAPIAPI.UpdateBooks(context.Background(), courseId).BookId(bookId).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `CourseAPIAPI.UpdateBooks``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `UpdateBooks`: Course
	fmt.Fprintf(os.Stdout, "Response from `CourseAPIAPI.UpdateBooks`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**courseId** | **string** | Course id |

### Other Parameters

Other parameters are passed through a pointer to a apiUpdateBooksRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **bookId** | **string** | Book id to process |

### Return type

[**Course**](Course.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data, application/x-www-form-urlencoded
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

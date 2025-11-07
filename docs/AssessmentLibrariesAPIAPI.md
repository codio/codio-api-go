# \AssessmentLibrariesAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**AssessmentLibraryCreateAssessment**](AssessmentLibrariesAPIAPI.md#AssessmentLibraryCreateAssessment) | **Post** /api/v1/assessment_library/{libraryId}/assessment | Create assessment
[**AssessmentLibraryGetAssessment**](AssessmentLibrariesAPIAPI.md#AssessmentLibraryGetAssessment) | **Get** /api/v1/assessment_library/{libraryId}/assessment/{id} | Get assessment
[**AssessmentLibrarySearch**](AssessmentLibrariesAPIAPI.md#AssessmentLibrarySearch) | **Get** /api/v1/assessment_library/{libraryId}/assessment | Search assessments
[**AssessmentLibraryUpdateAssessment**](AssessmentLibrariesAPIAPI.md#AssessmentLibraryUpdateAssessment) | **Put** /api/v1/assessment_library/{libraryId}/assessment/{id} | Update assessment
[**ListLibraries**](AssessmentLibrariesAPIAPI.md#ListLibraries) | **Get** /api/v1/assessment_library | List assessment libraries



## AssessmentLibraryCreateAssessment

> string AssessmentLibraryCreateAssessment(ctx, libraryId).Bundle(bundle).Assessment(assessment).Execute()

Create assessment

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
	libraryId := "libraryId_example" // string | Library id
	bundle := os.NewFile(1234, "some_file") // *os.File | Optional file archive data to be published (optional)
	assessment := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssessmentLibrariesAPIAPI.AssessmentLibraryCreateAssessment(context.Background(), libraryId).Bundle(bundle).Assessment(assessment).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssessmentLibrariesAPIAPI.AssessmentLibraryCreateAssessment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssessmentLibraryCreateAssessment`: string
	fmt.Fprintf(os.Stdout, "Response from `AssessmentLibrariesAPIAPI.AssessmentLibraryCreateAssessment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**libraryId** | **string** | Library id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssessmentLibraryCreateAssessmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **bundle** | ***os.File** | Optional file archive data to be published | 
 **assessment** | **map[string]interface{}** |  | 

### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AssessmentLibraryGetAssessment

> string AssessmentLibraryGetAssessment(ctx, libraryId, id).Execute()

Get assessment

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
	libraryId := "libraryId_example" // string | Library id
	id := "id_example" // string | Assessment id

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssessmentLibrariesAPIAPI.AssessmentLibraryGetAssessment(context.Background(), libraryId, id).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssessmentLibrariesAPIAPI.AssessmentLibraryGetAssessment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssessmentLibraryGetAssessment`: string
	fmt.Fprintf(os.Stdout, "Response from `AssessmentLibrariesAPIAPI.AssessmentLibraryGetAssessment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**libraryId** | **string** | Library id | 
**id** | **string** | Assessment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssessmentLibraryGetAssessmentRequest struct via the builder pattern


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


## AssessmentLibrarySearch

> SocrateAnswerExample AssessmentLibrarySearch(ctx, libraryId).Count(count).Offset(offset).Free(free).Execute()

Search assessments

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
	libraryId := "libraryId_example" // string | Library id
	count := "count_example" // string | Optional count parameter (optional)
	offset := "offset_example" // string | Optional offset parameter (optional)
	free := *openapiclient.NewSocrateTagSearchExample() // SocrateTagSearchExample | Free form tag search is allowed (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssessmentLibrariesAPIAPI.AssessmentLibrarySearch(context.Background(), libraryId).Count(count).Offset(offset).Free(free).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssessmentLibrariesAPIAPI.AssessmentLibrarySearch``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssessmentLibrarySearch`: SocrateAnswerExample
	fmt.Fprintf(os.Stdout, "Response from `AssessmentLibrariesAPIAPI.AssessmentLibrarySearch`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**libraryId** | **string** | Library id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssessmentLibrarySearchRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------

 **count** | **string** | Optional count parameter | 
 **offset** | **string** | Optional offset parameter | 
 **free** | [**SocrateTagSearchExample**](SocrateTagSearchExample.md) | Free form tag search is allowed | 

### Return type

[**SocrateAnswerExample**](SocrateAnswerExample.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## AssessmentLibraryUpdateAssessment

> string AssessmentLibraryUpdateAssessment(ctx, libraryId, id).Bundle(bundle).Assessment(assessment).Execute()

Update assessment

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
	libraryId := "libraryId_example" // string | Library id
	id := "id_example" // string | Assessment id
	bundle := os.NewFile(1234, "some_file") // *os.File | Optional file archive data to be published (optional)
	assessment := map[string]interface{}{"key": interface{}(123)} // map[string]interface{} |  (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssessmentLibrariesAPIAPI.AssessmentLibraryUpdateAssessment(context.Background(), libraryId, id).Bundle(bundle).Assessment(assessment).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssessmentLibrariesAPIAPI.AssessmentLibraryUpdateAssessment``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `AssessmentLibraryUpdateAssessment`: string
	fmt.Fprintf(os.Stdout, "Response from `AssessmentLibrariesAPIAPI.AssessmentLibraryUpdateAssessment`: %v\n", resp)
}
```

### Path Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
**ctx** | **context.Context** | context for authentication, logging, cancellation, deadlines, tracing, etc.
**libraryId** | **string** | Library id | 
**id** | **string** | Assessment id | 

### Other Parameters

Other parameters are passed through a pointer to a apiAssessmentLibraryUpdateAssessmentRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------


 **bundle** | ***os.File** | Optional file archive data to be published | 
 **assessment** | **map[string]interface{}** |  | 

### Return type

**string**

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: multipart/form-data, application/json
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## ListLibraries

> []SocratesLibrary ListLibraries(ctx).Execute()

List assessment libraries

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

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.AssessmentLibrariesAPIAPI.ListLibraries(context.Background()).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `AssessmentLibrariesAPIAPI.ListLibraries``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `ListLibraries`: []SocratesLibrary
	fmt.Fprintf(os.Stdout, "Response from `AssessmentLibrariesAPIAPI.ListLibraries`: %v\n", resp)
}
```

### Path Parameters

This endpoint does not need any parameter.

### Other Parameters

Other parameters are passed through a pointer to a apiListLibrariesRequest struct via the builder pattern


### Return type

[**[]SocratesLibrary**](SocratesLibrary.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


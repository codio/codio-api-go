# \EventsAPIAPI

All URIs are relative to *https://octopus.codio.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**EventList**](EventsAPIAPI.md#EventList) | **Get** /api/v1/events | List Webhook Events



## EventList

> EventsList EventList(ctx).NextToken(nextToken).Limit(limit).Execute()

List Webhook Events

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
	nextToken := "nextToken_example" // string | Continuation request token (optional)
	limit := "limit_example" // string | Count of returned events (optional)

	configuration := openapiclient.NewConfiguration()
	apiClient := openapiclient.NewAPIClient(configuration)
	resp, r, err := apiClient.EventsAPIAPI.EventList(context.Background()).NextToken(nextToken).Limit(limit).Execute()
	if err != nil {
		fmt.Fprintf(os.Stderr, "Error when calling `EventsAPIAPI.EventList``: %v\n", err)
		fmt.Fprintf(os.Stderr, "Full HTTP response: %v\n", r)
	}
	// response from `EventList`: EventsList
	fmt.Fprintf(os.Stdout, "Response from `EventsAPIAPI.EventList`: %v\n", resp)
}
```

### Path Parameters



### Other Parameters

Other parameters are passed through a pointer to a apiEventListRequest struct via the builder pattern


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **nextToken** | **string** | Continuation request token |
 **limit** | **string** | Count of returned events |

### Return type

[**EventsList**](EventsList.md)

### Authorization

[bearerAuth](../README.md#bearerAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

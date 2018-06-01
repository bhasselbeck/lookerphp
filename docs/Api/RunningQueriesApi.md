# Swagger\Client\RunningQueriesApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allRunningQueries**](RunningQueriesApi.md#allRunningQueries) | **GET** /running_queries | Get All Running Queries
[**killQuery**](RunningQueriesApi.md#killQuery) | **DELETE** /running_queries/{query_task_id} | Kill Running Query


# **allRunningQueries**
> \Swagger\Client\Looker\Model\RunningQueries[] allRunningQueries()

Get All Running Queries

Get information about all running queries.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\RunningQueriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);

try {
    $result = $apiInstance->allRunningQueries();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RunningQueriesApi->allRunningQueries: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**\Swagger\Client\Looker\Model\RunningQueries[]**](../Model/RunningQueries.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **killQuery**
> string killQuery($query_task_id)

Kill Running Query

Kill a query with a specific query_task_id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\RunningQueriesApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$query_task_id = "query_task_id_example"; // string | Query task id.

try {
    $result = $apiInstance->killQuery($query_task_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RunningQueriesApi->killQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **query_task_id** | **string**| Query task id. |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


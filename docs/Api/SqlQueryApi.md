# Looker\SqlQueryApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSqlQuery**](SqlQueryApi.md#createSqlQuery) | **POST** /sql_queries | Create SQL Runner Query
[**sqlQuery**](SqlQueryApi.md#sqlQuery) | **GET** /sql_queries/{slug} | Get SQL Runner Query


# **createSqlQuery**
> \Looker\Model\SqlQuery createSqlQuery($body)

Create SQL Runner Query

Create a SQL Runner query.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SqlQueryApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\SqlQueryCreate(); // \Looker\Model\SqlQueryCreate | SQL Runner Query

try {
    $result = $apiInstance->createSqlQuery($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SqlQueryApi->createSqlQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\SqlQueryCreate**](../Model/SqlQueryCreate.md)| SQL Runner Query |

### Return type

[**\Looker\Model\SqlQuery**](../Model/SqlQuery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sqlQuery**
> \Looker\Model\SqlQuery sqlQuery($slug)

Get SQL Runner Query

Get a SQL Runner query.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SqlQueryApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$slug = "slug_example"; // string | slug of query

try {
    $result = $apiInstance->sqlQuery($slug);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SqlQueryApi->sqlQuery: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **slug** | **string**| slug of query |

### Return type

[**\Looker\Model\SqlQuery**](../Model/SqlQuery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


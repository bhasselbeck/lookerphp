# Swagger\Client\LookApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allLooks**](LookApi.md#allLooks) | **GET** /looks | Get All Looks
[**createLook**](LookApi.md#createLook) | **POST** /looks | Create Look
[**deleteLook**](LookApi.md#deleteLook) | **DELETE** /looks/{look_id} | Delete Look
[**look**](LookApi.md#look) | **GET** /looks/{look_id} | Get Look
[**runLook**](LookApi.md#runLook) | **GET** /looks/{look_id}/run/{result_format} | Run Look
[**searchLooks**](LookApi.md#searchLooks) | **GET** /looks/search | Search Looks
[**updateLook**](LookApi.md#updateLook) | **PATCH** /looks/{look_id} | Update Look


# **allLooks**
> \Swagger\Client\Model\Look[] allLooks($fields)

Get All Looks

### Get all the looks.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allLooks($fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->allLooks: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\Look[]**](../Model/Look.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createLook**
> \Swagger\Client\Model\LookWithQuery createLook($body, $fields)

Create Look

### Create a Look with specified information.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\LookWithQuery(); // \Swagger\Client\Model\LookWithQuery | Look
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createLook($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->createLook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\LookWithQuery**](../Model/LookWithQuery.md)| Look | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\LookWithQuery**](../Model/LookWithQuery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteLook**
> string deleteLook($look_id)

Delete Look

### Delete the look with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$look_id = 789; // int | Id of look

try {
    $result = $apiInstance->deleteLook($look_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->deleteLook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **look_id** | **int**| Id of look |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **look**
> \Swagger\Client\Model\LookWithQuery look($look_id, $fields)

Get Look

### Get a Look.  Return detailed information about the Look and its associated Query.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$look_id = 789; // int | Id of look
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->look($look_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->look: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **look_id** | **int**| Id of look |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\LookWithQuery**](../Model/LookWithQuery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **runLook**
> string runLook($look_id, $result_format, $limit, $apply_formatting, $apply_vis, $cache, $image_width, $image_height, $generate_drill_links, $force_production, $cache_only, $path_prefix, $rebuild_pdts, $server_table_calcs)

Run Look

### Run a Look.  Runs a given look's query and returns the results in the requested format.  Suported formats:  | result_format | Description | :-----------: | :--- | | json | Plain json | json_detail | Row data plus metadata describing the fields, pivots, table calcs, and other aspects of the query | csv | Comma separated values with a header | txt | Tab separated values with a header | html | Simple html | md | Simple markdown | xlsx | MS Excel spreadsheet | sql | Returns the generated SQL rather than running the query | png | A PNG image of the visualization of the query | jpg | A JPG image of the visualization of the query

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$look_id = 789; // int | Id of look
$result_format = "result_format_example"; // string | Format of result
$limit = 789; // int | Row limit (may override the limit in the saved query).
$apply_formatting = true; // bool | Apply model-specified formatting to each result.
$apply_vis = true; // bool | Apply visualization options to results.
$cache = true; // bool | Get results from cache if available.
$image_width = 789; // int | Render width for image formats.
$image_height = 789; // int | Render height for image formats.
$generate_drill_links = true; // bool | Generate drill links (only applicable to 'json_detail' format.
$force_production = true; // bool | Force use of production models even if the user is in development mode.
$cache_only = true; // bool | Retrieve any results from cache even if the results have expired.
$path_prefix = "path_prefix_example"; // string | Prefix to use for drill links (url encoded).
$rebuild_pdts = true; // bool | Rebuild PDTS used in query.
$server_table_calcs = true; // bool | Perform table calculations on query results

try {
    $result = $apiInstance->runLook($look_id, $result_format, $limit, $apply_formatting, $apply_vis, $cache, $image_width, $image_height, $generate_drill_links, $force_production, $cache_only, $path_prefix, $rebuild_pdts, $server_table_calcs);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->runLook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **look_id** | **int**| Id of look |
 **result_format** | **string**| Format of result |
 **limit** | **int**| Row limit (may override the limit in the saved query). | [optional]
 **apply_formatting** | **bool**| Apply model-specified formatting to each result. | [optional]
 **apply_vis** | **bool**| Apply visualization options to results. | [optional]
 **cache** | **bool**| Get results from cache if available. | [optional]
 **image_width** | **int**| Render width for image formats. | [optional]
 **image_height** | **int**| Render height for image formats. | [optional]
 **generate_drill_links** | **bool**| Generate drill links (only applicable to &#39;json_detail&#39; format. | [optional]
 **force_production** | **bool**| Force use of production models even if the user is in development mode. | [optional]
 **cache_only** | **bool**| Retrieve any results from cache even if the results have expired. | [optional]
 **path_prefix** | **string**| Prefix to use for drill links (url encoded). | [optional]
 **rebuild_pdts** | **bool**| Rebuild PDTS used in query. | [optional]
 **server_table_calcs** | **bool**| Perform table calculations on query results | [optional]

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text, application/json, image/png, image/jpg

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchLooks**
> \Swagger\Client\Model\Look[] searchLooks($fields, $page, $per_page, $limit, $offset, $sorts, $title, $description, $content_favorite_id, $space_id, $user_id, $view_count)

Search Looks

Search looks.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$page = 789; // int | Requested page.
$per_page = 789; // int | Results per page.
$limit = 789; // int | Number of results to return. (used with offset and takes priority over page and per_page)
$offset = 789; // int | Number of results to skip before returning any. (used with limit and takes priority over page and per_page)
$sorts = "sorts_example"; // string | Fields to sort by.
$title = "title_example"; // string | Match Look title.
$description = "description_example"; // string | Match Look description.
$content_favorite_id = 789; // int | Match content favorite id
$space_id = "space_id_example"; // string | Filter on a particular space.
$user_id = "user_id_example"; // string | Filter on dashboards created by a particular user.
$view_count = "view_count_example"; // string | Filter on a particular value of view_count

try {
    $result = $apiInstance->searchLooks($fields, $page, $per_page, $limit, $offset, $sorts, $title, $description, $content_favorite_id, $space_id, $user_id, $view_count);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->searchLooks: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **page** | **int**| Requested page. | [optional]
 **per_page** | **int**| Results per page. | [optional]
 **limit** | **int**| Number of results to return. (used with offset and takes priority over page and per_page) | [optional]
 **offset** | **int**| Number of results to skip before returning any. (used with limit and takes priority over page and per_page) | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **title** | **string**| Match Look title. | [optional]
 **description** | **string**| Match Look description. | [optional]
 **content_favorite_id** | **int**| Match content favorite id | [optional]
 **space_id** | **string**| Filter on a particular space. | [optional]
 **user_id** | **string**| Filter on dashboards created by a particular user. | [optional]
 **view_count** | **string**| Filter on a particular value of view_count | [optional]

### Return type

[**\Swagger\Client\Model\Look[]**](../Model/Look.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateLook**
> \Swagger\Client\Model\LookWithQuery updateLook($look_id, $body, $fields)

Update Look

### Update the Look with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\LookApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$look_id = 789; // int | Id of look
$body = new \Swagger\Client\Model\LookWithQuery(); // \Swagger\Client\Model\LookWithQuery | Look
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateLook($look_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling LookApi->updateLook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **look_id** | **int**| Id of look |
 **body** | [**\Swagger\Client\Model\LookWithQuery**](../Model/LookWithQuery.md)| Look |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\LookWithQuery**](../Model/LookWithQuery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


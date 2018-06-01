# Looker\SpaceApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allSpaces**](SpaceApi.md#allSpaces) | **GET** /spaces | Get All Spaces
[**createSpace**](SpaceApi.md#createSpace) | **POST** /spaces | Create Space
[**deleteSpace**](SpaceApi.md#deleteSpace) | **DELETE** /spaces/{space_id} | Delete Space
[**searchSpaces**](SpaceApi.md#searchSpaces) | **GET** /spaces/search | Search Spaces
[**space**](SpaceApi.md#space) | **GET** /spaces/{space_id} | Get Space
[**spaceAncestors**](SpaceApi.md#spaceAncestors) | **GET** /spaces/{space_id}/ancestors | Get Space Ancestors
[**spaceChildren**](SpaceApi.md#spaceChildren) | **GET** /spaces/{space_id}/children | Get Space Children
[**spaceChildrenSearch**](SpaceApi.md#spaceChildrenSearch) | **GET** /spaces/{space_id}/children/search | Search Space Children
[**spaceDashboards**](SpaceApi.md#spaceDashboards) | **GET** /spaces/{space_id}/dashboards | Get Space Dashboards
[**spaceLooks**](SpaceApi.md#spaceLooks) | **GET** /spaces/{space_id}/looks | Get Space Looks
[**spaceParent**](SpaceApi.md#spaceParent) | **GET** /spaces/{space_id}/parent | Get Space Parent
[**updateSpace**](SpaceApi.md#updateSpace) | **PATCH** /spaces/{space_id} | Update Space


# **allSpaces**
> \Looker\Model\SpaceBase[] allSpaces($fields)

Get All Spaces

### Get information about all spaces.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allSpaces($fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->allSpaces: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\SpaceBase[]**](../Model/SpaceBase.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createSpace**
> \Looker\Model\Space createSpace($body)

Create Space

### Create a space with specified information.  Caller must have permission to edit the parent space and to create spaces, otherwise the request returns 404 Not Found.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\Space(); // \Looker\Model\Space | Space

try {
    $result = $apiInstance->createSpace($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->createSpace: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\Space**](../Model/Space.md)| Space | [optional]

### Return type

[**\Looker\Model\Space**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteSpace**
> string deleteSpace($space_id)

Delete Space

### Delete the space with a specific id including any children spaces. **DANGER** this will delete all looks and dashboards in the space.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space

try {
    $result = $apiInstance->deleteSpace($space_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->deleteSpace: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchSpaces**
> \Looker\Model\Space[] searchSpaces($fields, $page, $per_page, $limit, $offset, $sorts, $name, $id, $parent_id, $creator_id)

Search Spaces

Search for spaces by creator id, parent id, name, etc

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
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
$name = "name_example"; // string | Match Space title.
$id = 789; // int | Match Space id
$parent_id = "parent_id_example"; // string | Filter on a children of a particular space.
$creator_id = "creator_id_example"; // string | Filter on dashboards created by a particular user.

try {
    $result = $apiInstance->searchSpaces($fields, $page, $per_page, $limit, $offset, $sorts, $name, $id, $parent_id, $creator_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->searchSpaces: ', $e->getMessage(), PHP_EOL;
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
 **name** | **string**| Match Space title. | [optional]
 **id** | **int**| Match Space id | [optional]
 **parent_id** | **string**| Filter on a children of a particular space. | [optional]
 **creator_id** | **string**| Filter on dashboards created by a particular user. | [optional]

### Return type

[**\Looker\Model\Space[]**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **space**
> \Looker\Model\Space space($space_id, $fields)

Get Space

### Get information about the space with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->space($space_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->space: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\Space**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spaceAncestors**
> \Looker\Model\Space[] spaceAncestors($space_id, $fields)

Get Space Ancestors

### Get the ancestors of a space

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->spaceAncestors($space_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->spaceAncestors: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\Space[]**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spaceChildren**
> \Looker\Model\Space[] spaceChildren($space_id, $fields, $page, $per_page, $sorts)

Get Space Children

### Get the children of a space.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.
$page = 789; // int | Requested page.
$per_page = 789; // int | Results per page.
$sorts = "sorts_example"; // string | Fields to sort by.

try {
    $result = $apiInstance->spaceChildren($space_id, $fields, $page, $per_page, $sorts);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->spaceChildren: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]
 **page** | **int**| Requested page. | [optional]
 **per_page** | **int**| Results per page. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]

### Return type

[**\Looker\Model\Space[]**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spaceChildrenSearch**
> \Looker\Model\Space[] spaceChildrenSearch($space_id, $fields, $sorts, $name)

Search Space Children

### Search the children of a space

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.
$sorts = "sorts_example"; // string | Fields to sort by.
$name = "name_example"; // string | Match Space name.

try {
    $result = $apiInstance->spaceChildrenSearch($space_id, $fields, $sorts, $name);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->spaceChildrenSearch: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **name** | **string**| Match Space name. | [optional]

### Return type

[**\Looker\Model\Space[]**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spaceDashboards**
> \Looker\Model\Dashboard[] spaceDashboards($space_id, $fields)

Get Space Dashboards

### Get the dashboards in a space

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->spaceDashboards($space_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->spaceDashboards: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\Dashboard[]**](../Model/Dashboard.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spaceLooks**
> \Looker\Model\LookWithQuery[] spaceLooks($space_id, $fields)

Get Space Looks

### Get the looks in a space

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->spaceLooks($space_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->spaceLooks: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\LookWithQuery[]**](../Model/LookWithQuery.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **spaceParent**
> \Looker\Model\Space spaceParent($space_id, $fields)

Get Space Parent

### Get the parent of a space

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->spaceParent($space_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->spaceParent: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\Space**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateSpace**
> \Looker\Model\Space updateSpace($space_id, $body)

Update Space

### Update the space with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\SpaceApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = "space_id_example"; // string | Id of space
$body = new \Looker\Model\Space(); // \Looker\Model\Space | Space

try {
    $result = $apiInstance->updateSpace($space_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SpaceApi->updateSpace: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **string**| Id of space |
 **body** | [**\Looker\Model\Space**](../Model/Space.md)| Space |

### Return type

[**\Looker\Model\Space**](../Model/Space.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


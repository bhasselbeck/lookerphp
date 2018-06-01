# Looker\HomepageApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allHomepageItems**](HomepageApi.md#allHomepageItems) | **GET** /homepage_items | Get All Homepage Items
[**allHomepageSections**](HomepageApi.md#allHomepageSections) | **GET** /homepage_sections | Get All Homepage sections
[**createHomepageItem**](HomepageApi.md#createHomepageItem) | **POST** /homepage_items | Create Homepage Item
[**createHomepageSection**](HomepageApi.md#createHomepageSection) | **POST** /homepage_sections | Create Homepage section
[**deleteHomepageItem**](HomepageApi.md#deleteHomepageItem) | **DELETE** /homepage_items/{homepage_item_id} | Delete Homepage Item
[**deleteHomepageSection**](HomepageApi.md#deleteHomepageSection) | **DELETE** /homepage_sections/{homepage_section_id} | Delete Homepage section
[**homepageItem**](HomepageApi.md#homepageItem) | **GET** /homepage_items/{homepage_item_id} | Get Homepage Item
[**homepageSection**](HomepageApi.md#homepageSection) | **GET** /homepage_sections/{homepage_section_id} | Get Homepage section
[**updateHomepageItem**](HomepageApi.md#updateHomepageItem) | **PATCH** /homepage_items/{homepage_item_id} | Update Homepage Item
[**updateHomepageSection**](HomepageApi.md#updateHomepageSection) | **PATCH** /homepage_sections/{homepage_section_id} | Update Homepage section


# **allHomepageItems**
> \Looker\Model\HomepageItem[] allHomepageItems($fields, $sorts, $homepage_section_id)

Get All Homepage Items

### Get information about all homepage items.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$sorts = "sorts_example"; // string | Fields to sort by.
$homepage_section_id = "homepage_section_id_example"; // string | Filter to a specific homepage section

try {
    $result = $apiInstance->allHomepageItems($fields, $sorts, $homepage_section_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->allHomepageItems: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **homepage_section_id** | **string**| Filter to a specific homepage section | [optional]

### Return type

[**\Looker\Model\HomepageItem[]**](../Model/HomepageItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allHomepageSections**
> \Looker\Model\HomepageSection[] allHomepageSections($fields, $sorts)

Get All Homepage sections

### Get information about all homepage sections.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$sorts = "sorts_example"; // string | Fields to sort by.

try {
    $result = $apiInstance->allHomepageSections($fields, $sorts);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->allHomepageSections: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]

### Return type

[**\Looker\Model\HomepageSection[]**](../Model/HomepageSection.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createHomepageItem**
> \Looker\Model\HomepageItem createHomepageItem($body, $fields)

Create Homepage Item

### Create a new homepage item.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\HomepageItem(); // \Looker\Model\HomepageItem | Homepage Item
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createHomepageItem($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->createHomepageItem: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\HomepageItem**](../Model/HomepageItem.md)| Homepage Item | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\HomepageItem**](../Model/HomepageItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createHomepageSection**
> \Looker\Model\HomepageSection createHomepageSection($body, $fields)

Create Homepage section

### Create a new homepage section.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\HomepageSection(); // \Looker\Model\HomepageSection | Homepage section
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createHomepageSection($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->createHomepageSection: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\HomepageSection**](../Model/HomepageSection.md)| Homepage section | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\HomepageSection**](../Model/HomepageSection.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteHomepageItem**
> string deleteHomepageItem($homepage_item_id)

Delete Homepage Item

### Delete a homepage item.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$homepage_item_id = 789; // int | Id of homepage_item

try {
    $result = $apiInstance->deleteHomepageItem($homepage_item_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->deleteHomepageItem: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homepage_item_id** | **int**| Id of homepage_item |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteHomepageSection**
> string deleteHomepageSection($homepage_section_id)

Delete Homepage section

### Delete a homepage section.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$homepage_section_id = 789; // int | Id of homepage_section

try {
    $result = $apiInstance->deleteHomepageSection($homepage_section_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->deleteHomepageSection: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homepage_section_id** | **int**| Id of homepage_section |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **homepageItem**
> \Looker\Model\HomepageItem homepageItem($homepage_item_id, $fields)

Get Homepage Item

### Get information about a homepage item.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$homepage_item_id = 789; // int | Id of homepage item
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->homepageItem($homepage_item_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->homepageItem: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homepage_item_id** | **int**| Id of homepage item |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\HomepageItem**](../Model/HomepageItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **homepageSection**
> \Looker\Model\HomepageSection homepageSection($homepage_section_id, $fields)

Get Homepage section

### Get information about a homepage section.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$homepage_section_id = 789; // int | Id of homepage section
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->homepageSection($homepage_section_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->homepageSection: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homepage_section_id** | **int**| Id of homepage section |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\HomepageSection**](../Model/HomepageSection.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateHomepageItem**
> \Looker\Model\HomepageItem updateHomepageItem($homepage_item_id, $body, $fields)

Update Homepage Item

### Update a homepage item definition.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$homepage_item_id = 789; // int | Id of homepage item
$body = new \Looker\Model\HomepageItem(); // \Looker\Model\HomepageItem | Homepage Item
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateHomepageItem($homepage_item_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->updateHomepageItem: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homepage_item_id** | **int**| Id of homepage item |
 **body** | [**\Looker\Model\HomepageItem**](../Model/HomepageItem.md)| Homepage Item |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\HomepageItem**](../Model/HomepageItem.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateHomepageSection**
> \Looker\Model\HomepageSection updateHomepageSection($homepage_section_id, $body, $fields)

Update Homepage section

### Update a homepage section definition.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\HomepageApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$homepage_section_id = 789; // int | Id of homepage section
$body = new \Looker\Model\HomepageSection(); // \Looker\Model\HomepageSection | Homepage section
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateHomepageSection($homepage_section_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling HomepageApi->updateHomepageSection: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **homepage_section_id** | **int**| Id of homepage section |
 **body** | [**\Looker\Model\HomepageSection**](../Model/HomepageSection.md)| Homepage section |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\HomepageSection**](../Model/HomepageSection.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# Looker\ContentApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allContentMetadataAccesss**](ContentApi.md#allContentMetadataAccesss) | **GET** /content_metadata_access | Get All Content Metadata Accesss
[**allContentMetadatas**](ContentApi.md#allContentMetadatas) | **GET** /content_metadata | Get All Content Metadatas
[**contentFavorite**](ContentApi.md#contentFavorite) | **GET** /content_favorite/{content_favorite_id} | Get Favorite Content
[**contentMetadata**](ContentApi.md#contentMetadata) | **GET** /content_metadata/{content_metadata_id} | Get Content Metadata
[**createContentFavorite**](ContentApi.md#createContentFavorite) | **POST** /content_favorite | Create Favorite Content
[**createContentMetadataAccess**](ContentApi.md#createContentMetadataAccess) | **POST** /content_metadata_access | Create Content Metadata Access
[**deleteContentFavorite**](ContentApi.md#deleteContentFavorite) | **DELETE** /content_favorite/{content_favorite_id} | Delete Favorite Content
[**deleteContentMetadataAccess**](ContentApi.md#deleteContentMetadataAccess) | **DELETE** /content_metadata_access/{content_metadata_access_id} | Delete Content Metadata Access
[**searchContentFavorites**](ContentApi.md#searchContentFavorites) | **GET** /content_favorite/search | Search Favorite Contents
[**searchContentViews**](ContentApi.md#searchContentViews) | **GET** /content_view/search | Search Content Views
[**updateContentMetadata**](ContentApi.md#updateContentMetadata) | **PATCH** /content_metadata/{content_metadata_id} | Update Content Metadata
[**updateContentMetadataAccess**](ContentApi.md#updateContentMetadataAccess) | **PUT** /content_metadata_access/{content_metadata_access_id} | Update Content Metadata Access


# **allContentMetadataAccesss**
> \Looker\Model\ContentMetaGroupUser[] allContentMetadataAccesss($content_metadata_id, $fields)

Get All Content Metadata Accesss

### All content metadata access records for a content metadata item.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_metadata_id = 789; // int | Id of content metadata
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allContentMetadataAccesss($content_metadata_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->allContentMetadataAccesss: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_metadata_id** | **int**| Id of content metadata | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\ContentMetaGroupUser[]**](../Model/ContentMetaGroupUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allContentMetadatas**
> \Looker\Model\ContentMeta[] allContentMetadatas($parent_id, $fields)

Get All Content Metadatas

### Get information about all content metadata in a space.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$parent_id = 789; // int | Parent space of content.
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allContentMetadatas($parent_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->allContentMetadatas: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **parent_id** | **int**| Parent space of content. |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\ContentMeta[]**](../Model/ContentMeta.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **contentFavorite**
> \Looker\Model\ContentFavorite contentFavorite($content_favorite_id, $fields)

Get Favorite Content

### Get favorite content by its id

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_favorite_id = 789; // int | Id of favorite content
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->contentFavorite($content_favorite_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->contentFavorite: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_favorite_id** | **int**| Id of favorite content |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\ContentFavorite**](../Model/ContentFavorite.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **contentMetadata**
> \Looker\Model\ContentMeta contentMetadata($content_metadata_id, $fields)

Get Content Metadata

### Get information about an individual content metadata record.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_metadata_id = 789; // int | Id of content metadata
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->contentMetadata($content_metadata_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->contentMetadata: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_metadata_id** | **int**| Id of content metadata |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\ContentMeta**](../Model/ContentMeta.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createContentFavorite**
> \Looker\Model\ContentFavorite createContentFavorite($body)

Create Favorite Content

### Create favorite content

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\ContentFavorite(); // \Looker\Model\ContentFavorite | Favorite Content

try {
    $result = $apiInstance->createContentFavorite($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->createContentFavorite: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\ContentFavorite**](../Model/ContentFavorite.md)| Favorite Content | [optional]

### Return type

[**\Looker\Model\ContentFavorite**](../Model/ContentFavorite.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createContentMetadataAccess**
> \Looker\Model\ContentMetaGroupUser createContentMetadataAccess($body)

Create Content Metadata Access

### Create content metadata access.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\ContentMetaGroupUser(); // \Looker\Model\ContentMetaGroupUser | Content Metadata Access

try {
    $result = $apiInstance->createContentMetadataAccess($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->createContentMetadataAccess: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\ContentMetaGroupUser**](../Model/ContentMetaGroupUser.md)| Content Metadata Access | [optional]

### Return type

[**\Looker\Model\ContentMetaGroupUser**](../Model/ContentMetaGroupUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteContentFavorite**
> string deleteContentFavorite($content_favorite_id)

Delete Favorite Content

### Delete favorite content

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_favorite_id = 789; // int | Id of favorite content

try {
    $result = $apiInstance->deleteContentFavorite($content_favorite_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->deleteContentFavorite: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_favorite_id** | **int**| Id of favorite content |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteContentMetadataAccess**
> string deleteContentMetadataAccess($content_metadata_access_id)

Delete Content Metadata Access

### Remove content metadata access.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_metadata_access_id = 789; // int | Id of content metadata access

try {
    $result = $apiInstance->deleteContentMetadataAccess($content_metadata_access_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->deleteContentMetadataAccess: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_metadata_access_id** | **int**| Id of content metadata access |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchContentFavorites**
> \Looker\Model\ContentFavorite[] searchContentFavorites($user_id, $limit, $offset, $sorts, $fields)

Search Favorite Contents

### Search Favorite Content

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Match User Id
$limit = 789; // int | Number of results to return. (used with offset)
$offset = 789; // int | Number of results to skip before returning any. (used with limit)
$sorts = "sorts_example"; // string | Fields to sort by.
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->searchContentFavorites($user_id, $limit, $offset, $sorts, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->searchContentFavorites: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Match User Id | [optional]
 **limit** | **int**| Number of results to return. (used with offset) | [optional]
 **offset** | **int**| Number of results to skip before returning any. (used with limit) | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\ContentFavorite[]**](../Model/ContentFavorite.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchContentViews**
> \Looker\Model\ContentView[] searchContentViews($view_count, $group_id, $look_id, $dashboard_id, $content_metadata_id, $start_of_week_date, $all_time, $user_id, $limit, $offset, $sorts, $fields)

Search Content Views

### Search Content View

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$view_count = 789; // int | Match view count
$group_id = 789; // int | Match Group Id
$look_id = "look_id_example"; // string | Match look_id
$dashboard_id = "dashboard_id_example"; // string | Match dashboard_id
$content_metadata_id = 789; // int | Match content metadata id
$start_of_week_date = "start_of_week_date_example"; // string | Match start of week date
$all_time = true; // bool | True if only all time view records should be returned
$user_id = 789; // int | Match user id
$limit = 789; // int | Number of results to return. Use with `offset` to manage pagination of results
$offset = 789; // int | Number of results to skip before returning data
$sorts = "sorts_example"; // string | Fields to sort by
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->searchContentViews($view_count, $group_id, $look_id, $dashboard_id, $content_metadata_id, $start_of_week_date, $all_time, $user_id, $limit, $offset, $sorts, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->searchContentViews: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **view_count** | **int**| Match view count | [optional]
 **group_id** | **int**| Match Group Id | [optional]
 **look_id** | **string**| Match look_id | [optional]
 **dashboard_id** | **string**| Match dashboard_id | [optional]
 **content_metadata_id** | **int**| Match content metadata id | [optional]
 **start_of_week_date** | **string**| Match start of week date | [optional]
 **all_time** | **bool**| True if only all time view records should be returned | [optional]
 **user_id** | **int**| Match user id | [optional]
 **limit** | **int**| Number of results to return. Use with &#x60;offset&#x60; to manage pagination of results | [optional]
 **offset** | **int**| Number of results to skip before returning data | [optional]
 **sorts** | **string**| Fields to sort by | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\ContentView[]**](../Model/ContentView.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateContentMetadata**
> \Looker\Model\ContentMeta updateContentMetadata($content_metadata_id, $body)

Update Content Metadata

### Move a piece of content.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_metadata_id = 789; // int | Id of content metadata
$body = new \Looker\Model\ContentMeta(); // \Looker\Model\ContentMeta | Content Metadata

try {
    $result = $apiInstance->updateContentMetadata($content_metadata_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->updateContentMetadata: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_metadata_id** | **int**| Id of content metadata |
 **body** | [**\Looker\Model\ContentMeta**](../Model/ContentMeta.md)| Content Metadata |

### Return type

[**\Looker\Model\ContentMeta**](../Model/ContentMeta.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateContentMetadataAccess**
> \Looker\Model\ContentMetaGroupUser updateContentMetadataAccess($content_metadata_access_id, $body)

Update Content Metadata Access

### Update type of access for content metadata.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\ContentApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$content_metadata_access_id = 789; // int | Id of content metadata access
$body = new \Looker\Model\ContentMetaGroupUser(); // \Looker\Model\ContentMetaGroupUser | Content Metadata Access

try {
    $result = $apiInstance->updateContentMetadataAccess($content_metadata_access_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ContentApi->updateContentMetadataAccess: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **content_metadata_access_id** | **int**| Id of content metadata access |
 **body** | [**\Looker\Model\ContentMetaGroupUser**](../Model/ContentMetaGroupUser.md)| Content Metadata Access |

### Return type

[**\Looker\Model\ContentMetaGroupUser**](../Model/ContentMetaGroupUser.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# Looker\DashboardApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allDashboards**](DashboardApi.md#allDashboards) | **GET** /dashboards | Get All Dashboards
[**createDashboard**](DashboardApi.md#createDashboard) | **POST** /dashboards | Create Dashboard
[**createDashboardElement**](DashboardApi.md#createDashboardElement) | **POST** /dashboard_elements | Create DashboardElement
[**createDashboardFilter**](DashboardApi.md#createDashboardFilter) | **POST** /dashboard_filters | Create Dashboard Filter
[**createDashboardLayout**](DashboardApi.md#createDashboardLayout) | **POST** /dashboard_layouts | Create DashboardLayout
[**dashboard**](DashboardApi.md#dashboard) | **GET** /dashboards/{dashboard_id} | Get Dashboard
[**dashboardDashboardElements**](DashboardApi.md#dashboardDashboardElements) | **GET** /dashboards/{dashboard_id}/dashboard_elements | Get All DashboardElements
[**dashboardDashboardFilters**](DashboardApi.md#dashboardDashboardFilters) | **GET** /dashboards/{dashboard_id}/dashboard_filters | Get All Dashboard Filters
[**dashboardDashboardLayouts**](DashboardApi.md#dashboardDashboardLayouts) | **GET** /dashboards/{dashboard_id}/dashboard_layouts | Get All DashboardLayouts
[**dashboardElement**](DashboardApi.md#dashboardElement) | **GET** /dashboard_elements/{dashboard_element_id} | Get DashboardElement
[**dashboardFilter**](DashboardApi.md#dashboardFilter) | **GET** /dashboard_filters/{dashboard_filter_id} | Get Dashboard Filter
[**dashboardLayout**](DashboardApi.md#dashboardLayout) | **GET** /dashboard_layouts/{dashboard_layout_id} | Get DashboardLayout
[**dashboardLayoutComponent**](DashboardApi.md#dashboardLayoutComponent) | **GET** /dashboard_layout_components/{dashboard_layout_component_id} | Get DashboardLayoutComponent
[**dashboardLayoutDashboardLayoutComponents**](DashboardApi.md#dashboardLayoutDashboardLayoutComponents) | **GET** /dashboard_layouts/{dashboard_layout_id}/dashboard_layout_components | Get All DashboardLayoutComponents
[**deleteDashboard**](DashboardApi.md#deleteDashboard) | **DELETE** /dashboards/{dashboard_id} | Delete Dashboard
[**deleteDashboardElement**](DashboardApi.md#deleteDashboardElement) | **DELETE** /dashboard_elements/{dashboard_element_id} | Delete DashboardElement
[**deleteDashboardFilter**](DashboardApi.md#deleteDashboardFilter) | **DELETE** /dashboard_filters/{dashboard_filter_id} | Delete Dashboard Filter
[**deleteDashboardLayout**](DashboardApi.md#deleteDashboardLayout) | **DELETE** /dashboard_layouts/{dashboard_layout_id} | Delete DashboardLayout
[**searchDashboardElements**](DashboardApi.md#searchDashboardElements) | **GET** /dashboard_elements/search | Get DashboardElement
[**searchDashboards**](DashboardApi.md#searchDashboards) | **GET** /dashboards/search | Search Dashboards
[**updateDashboard**](DashboardApi.md#updateDashboard) | **PATCH** /dashboards/{dashboard_id} | Update Dashboard
[**updateDashboardElement**](DashboardApi.md#updateDashboardElement) | **PATCH** /dashboard_elements/{dashboard_element_id} | Update DashboardElement
[**updateDashboardFilter**](DashboardApi.md#updateDashboardFilter) | **PATCH** /dashboard_filters/{dashboard_filter_id} | Update Dashboard Filter
[**updateDashboardLayout**](DashboardApi.md#updateDashboardLayout) | **PATCH** /dashboard_layouts/{dashboard_layout_id} | Update DashboardLayout
[**updateDashboardLayoutComponent**](DashboardApi.md#updateDashboardLayoutComponent) | **PATCH** /dashboard_layout_components/{dashboard_layout_component_id} | Update DashboardLayoutComponent


# **allDashboards**
> \Looker\Model\DashboardBase[] allDashboards($fields)

Get All Dashboards

Get information about all dashboards.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allDashboards($fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->allDashboards: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardBase[]**](../Model/DashboardBase.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createDashboard**
> \Looker\Model\Dashboard createDashboard($body)

Create Dashboard

### Create a dashboard with specified information.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\Dashboard(); // \Looker\Model\Dashboard | Dashboard

try {
    $result = $apiInstance->createDashboard($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->createDashboard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\Dashboard**](../Model/Dashboard.md)| Dashboard | [optional]

### Return type

[**\Looker\Model\Dashboard**](../Model/Dashboard.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createDashboardElement**
> \Looker\Model\DashboardElement createDashboardElement($body, $fields)

Create DashboardElement

### Create a dashboard element on the dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\DashboardElement(); // \Looker\Model\DashboardElement | DashboardElement
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createDashboardElement($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->createDashboardElement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\DashboardElement**](../Model/DashboardElement.md)| DashboardElement | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardElement**](../Model/DashboardElement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createDashboardFilter**
> \Looker\Model\DashboardFilter createDashboardFilter($body, $fields)

Create Dashboard Filter

### Create a dashboard filter on the dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\DashboardFilter(); // \Looker\Model\DashboardFilter | Dashboard Filter
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createDashboardFilter($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->createDashboardFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\DashboardFilter**](../Model/DashboardFilter.md)| Dashboard Filter | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardFilter**](../Model/DashboardFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createDashboardLayout**
> \Looker\Model\DashboardLayout createDashboardLayout($body, $fields)

Create DashboardLayout

### Create a dashboard layout on the dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\DashboardLayout(); // \Looker\Model\DashboardLayout | DashboardLayout
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createDashboardLayout($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->createDashboardLayout: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\DashboardLayout**](../Model/DashboardLayout.md)| DashboardLayout | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayout**](../Model/DashboardLayout.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboard**
> \Looker\Model\Dashboard dashboard($dashboard_id, $fields)

Get Dashboard

### Get information about the dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = "dashboard_id_example"; // string | Id of dashboard
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboard($dashboard_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **string**| Id of dashboard |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\Dashboard**](../Model/Dashboard.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardDashboardElements**
> \Looker\Model\DashboardElement[] dashboardDashboardElements($dashboard_id, $fields)

Get All DashboardElements

### Get information about all the dashboard elements on a dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = "dashboard_id_example"; // string | Id of dashboard
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardDashboardElements($dashboard_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardDashboardElements: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **string**| Id of dashboard |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardElement[]**](../Model/DashboardElement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardDashboardFilters**
> \Looker\Model\DashboardFilter[] dashboardDashboardFilters($dashboard_id, $fields)

Get All Dashboard Filters

### Get information about all the dashboard filters on a dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = "dashboard_id_example"; // string | Id of dashboard
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardDashboardFilters($dashboard_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardDashboardFilters: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **string**| Id of dashboard |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardFilter[]**](../Model/DashboardFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardDashboardLayouts**
> \Looker\Model\DashboardLayout[] dashboardDashboardLayouts($dashboard_id, $fields)

Get All DashboardLayouts

### Get information about all the dashboard elemnts on a dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = "dashboard_id_example"; // string | Id of dashboard
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardDashboardLayouts($dashboard_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardDashboardLayouts: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **string**| Id of dashboard |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayout[]**](../Model/DashboardLayout.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardElement**
> \Looker\Model\DashboardElement dashboardElement($dashboard_element_id, $fields)

Get DashboardElement

### Get information about the dashboard element with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_element_id = "dashboard_element_id_example"; // string | Id of dashboard element
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardElement($dashboard_element_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardElement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_element_id** | **string**| Id of dashboard element |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardElement**](../Model/DashboardElement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardFilter**
> \Looker\Model\DashboardFilter dashboardFilter($dashboard_filter_id, $fields)

Get Dashboard Filter

### Get information about the dashboard filters with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_filter_id = "dashboard_filter_id_example"; // string | Id of dashboard filters
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardFilter($dashboard_filter_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_filter_id** | **string**| Id of dashboard filters |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardFilter**](../Model/DashboardFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardLayout**
> \Looker\Model\DashboardLayout dashboardLayout($dashboard_layout_id, $fields)

Get DashboardLayout

### Get information about the dashboard layouts with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_layout_id = "dashboard_layout_id_example"; // string | Id of dashboard layouts
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardLayout($dashboard_layout_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardLayout: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_layout_id** | **string**| Id of dashboard layouts |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayout**](../Model/DashboardLayout.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardLayoutComponent**
> \Looker\Model\DashboardLayoutComponent dashboardLayoutComponent($dashboard_layout_component_id, $fields)

Get DashboardLayoutComponent

### Get information about the dashboard elements with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_layout_component_id = "dashboard_layout_component_id_example"; // string | Id of dashboard layout component
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardLayoutComponent($dashboard_layout_component_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardLayoutComponent: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_layout_component_id** | **string**| Id of dashboard layout component |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayoutComponent**](../Model/DashboardLayoutComponent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **dashboardLayoutDashboardLayoutComponents**
> \Looker\Model\DashboardLayoutComponent[] dashboardLayoutDashboardLayoutComponents($dashboard_layout_id, $fields)

Get All DashboardLayoutComponents

### Get information about all the dashboard layout components for a dashboard layout with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_layout_id = "dashboard_layout_id_example"; // string | Id of dashboard layout component
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->dashboardLayoutDashboardLayoutComponents($dashboard_layout_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->dashboardLayoutDashboardLayoutComponents: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_layout_id** | **string**| Id of dashboard layout component |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayoutComponent[]**](../Model/DashboardLayoutComponent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDashboard**
> string deleteDashboard($dashboard_id)

Delete Dashboard

### Delete the dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = "dashboard_id_example"; // string | Id of dashboard

try {
    $result = $apiInstance->deleteDashboard($dashboard_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->deleteDashboard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **string**| Id of dashboard |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDashboardElement**
> string deleteDashboardElement($dashboard_element_id)

Delete DashboardElement

### Delete a dashboard element with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_element_id = "dashboard_element_id_example"; // string | Id of dashboard element

try {
    $result = $apiInstance->deleteDashboardElement($dashboard_element_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->deleteDashboardElement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_element_id** | **string**| Id of dashboard element |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDashboardFilter**
> string deleteDashboardFilter($dashboard_filter_id)

Delete Dashboard Filter

### Delete a dashboard filter with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_filter_id = "dashboard_filter_id_example"; // string | Id of dashboard filter

try {
    $result = $apiInstance->deleteDashboardFilter($dashboard_filter_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->deleteDashboardFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_filter_id** | **string**| Id of dashboard filter |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteDashboardLayout**
> string deleteDashboardLayout($dashboard_layout_id)

Delete DashboardLayout

### Delete a dashboard layout with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_layout_id = "dashboard_layout_id_example"; // string | Id of dashboard layout

try {
    $result = $apiInstance->deleteDashboardLayout($dashboard_layout_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->deleteDashboardLayout: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_layout_id** | **string**| Id of dashboard layout |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchDashboardElements**
> \Looker\Model\DashboardElement[] searchDashboardElements($fields, $look_id, $dashboard_id, $title)

Get DashboardElement

### Get information on dashboard look relations for a set of look ids.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$look_id = 789; // int | Id of look
$dashboard_id = 789; // int | Id of dashboard
$title = "title_example"; // string | Title of element

try {
    $result = $apiInstance->searchDashboardElements($fields, $look_id, $dashboard_id, $title);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->searchDashboardElements: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **look_id** | **int**| Id of look | [optional]
 **dashboard_id** | **int**| Id of dashboard | [optional]
 **title** | **string**| Title of element | [optional]

### Return type

[**\Looker\Model\DashboardElement[]**](../Model/DashboardElement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchDashboards**
> \Looker\Model\Dashboard[] searchDashboards($fields, $id, $page, $per_page, $limit, $offset, $sorts, $title, $description, $content_favorite_id, $space_id, $deleted, $user_id, $view_count)

Search Dashboards

Get information about all dashboards.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$id = 789; // int | Match dashboard id.
$page = 789; // int | Requested page.
$per_page = 789; // int | Results per page.
$limit = 789; // int | Number of results to return. (used with offset and takes priority over page and per_page)
$offset = 789; // int | Number of results to skip before returning any. (used with limit and takes priority over page and per_page)
$sorts = "sorts_example"; // string | Fields to sort by.
$title = "title_example"; // string | Match Dashboard title.
$description = "description_example"; // string | Match Dashboard description.
$content_favorite_id = 789; // int | Filter on a content favorite id.
$space_id = "space_id_example"; // string | Filter on a particular space.
$deleted = "deleted_example"; // string | Filter on dashboards deleted status.
$user_id = "user_id_example"; // string | Filter on dashboards created by a particular user.
$view_count = "view_count_example"; // string | Filter on a particular value of view_count

try {
    $result = $apiInstance->searchDashboards($fields, $id, $page, $per_page, $limit, $offset, $sorts, $title, $description, $content_favorite_id, $space_id, $deleted, $user_id, $view_count);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->searchDashboards: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **id** | **int**| Match dashboard id. | [optional]
 **page** | **int**| Requested page. | [optional]
 **per_page** | **int**| Results per page. | [optional]
 **limit** | **int**| Number of results to return. (used with offset and takes priority over page and per_page) | [optional]
 **offset** | **int**| Number of results to skip before returning any. (used with limit and takes priority over page and per_page) | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **title** | **string**| Match Dashboard title. | [optional]
 **description** | **string**| Match Dashboard description. | [optional]
 **content_favorite_id** | **int**| Filter on a content favorite id. | [optional]
 **space_id** | **string**| Filter on a particular space. | [optional]
 **deleted** | **string**| Filter on dashboards deleted status. | [optional]
 **user_id** | **string**| Filter on dashboards created by a particular user. | [optional]
 **view_count** | **string**| Filter on a particular value of view_count | [optional]

### Return type

[**\Looker\Model\Dashboard[]**](../Model/Dashboard.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateDashboard**
> \Looker\Model\Dashboard updateDashboard($dashboard_id, $body)

Update Dashboard

### Update the dashboard with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = "dashboard_id_example"; // string | Id of dashboard
$body = new \Looker\Model\Dashboard(); // \Looker\Model\Dashboard | Dashboard

try {
    $result = $apiInstance->updateDashboard($dashboard_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->updateDashboard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **string**| Id of dashboard |
 **body** | [**\Looker\Model\Dashboard**](../Model/Dashboard.md)| Dashboard |

### Return type

[**\Looker\Model\Dashboard**](../Model/Dashboard.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateDashboardElement**
> \Looker\Model\DashboardElement updateDashboardElement($dashboard_element_id, $body, $fields)

Update DashboardElement

### Update the dashboard element with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_element_id = "dashboard_element_id_example"; // string | Id of dashboard element
$body = new \Looker\Model\DashboardElement(); // \Looker\Model\DashboardElement | DashboardElement
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateDashboardElement($dashboard_element_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->updateDashboardElement: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_element_id** | **string**| Id of dashboard element |
 **body** | [**\Looker\Model\DashboardElement**](../Model/DashboardElement.md)| DashboardElement |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardElement**](../Model/DashboardElement.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateDashboardFilter**
> \Looker\Model\DashboardFilter updateDashboardFilter($dashboard_filter_id, $body, $fields)

Update Dashboard Filter

### Update the dashboard filter with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_filter_id = "dashboard_filter_id_example"; // string | Id of dashboard filter
$body = new \Looker\Model\DashboardFilter(); // \Looker\Model\DashboardFilter | Dashboard Filter
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateDashboardFilter($dashboard_filter_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->updateDashboardFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_filter_id** | **string**| Id of dashboard filter |
 **body** | [**\Looker\Model\DashboardFilter**](../Model/DashboardFilter.md)| Dashboard Filter |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardFilter**](../Model/DashboardFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateDashboardLayout**
> \Looker\Model\DashboardLayout updateDashboardLayout($dashboard_layout_id, $body, $fields)

Update DashboardLayout

### Update the dashboard layout with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_layout_id = "dashboard_layout_id_example"; // string | Id of dashboard layout
$body = new \Looker\Model\DashboardLayout(); // \Looker\Model\DashboardLayout | DashboardLayout
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateDashboardLayout($dashboard_layout_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->updateDashboardLayout: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_layout_id** | **string**| Id of dashboard layout |
 **body** | [**\Looker\Model\DashboardLayout**](../Model/DashboardLayout.md)| DashboardLayout |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayout**](../Model/DashboardLayout.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateDashboardLayoutComponent**
> \Looker\Model\DashboardLayoutComponent updateDashboardLayoutComponent($dashboard_layout_component_id, $body, $fields)

Update DashboardLayoutComponent

### Update the dashboard element with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\DashboardApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_layout_component_id = "dashboard_layout_component_id_example"; // string | Id of dashboard layout component
$body = new \Looker\Model\DashboardLayoutComponent(); // \Looker\Model\DashboardLayoutComponent | DashboardLayoutComponent
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateDashboardLayoutComponent($dashboard_layout_component_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling DashboardApi->updateDashboardLayoutComponent: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_layout_component_id** | **string**| Id of dashboard layout component |
 **body** | [**\Looker\Model\DashboardLayoutComponent**](../Model/DashboardLayoutComponent.md)| DashboardLayoutComponent |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\DashboardLayoutComponent**](../Model/DashboardLayoutComponent.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


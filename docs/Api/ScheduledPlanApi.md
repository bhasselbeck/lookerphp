# Swagger\Client\ScheduledPlanApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allScheduledPlans**](ScheduledPlanApi.md#allScheduledPlans) | **GET** /scheduled_plans | Get All Scheduled Plans
[**createScheduledPlan**](ScheduledPlanApi.md#createScheduledPlan) | **POST** /scheduled_plans | Create Scheduled Plan
[**deleteScheduledPlan**](ScheduledPlanApi.md#deleteScheduledPlan) | **DELETE** /scheduled_plans/{scheduled_plan_id} | Delete Scheduled Plan
[**scheduledPlan**](ScheduledPlanApi.md#scheduledPlan) | **GET** /scheduled_plans/{scheduled_plan_id} | Get Scheduled Plan
[**scheduledPlanRunOnce**](ScheduledPlanApi.md#scheduledPlanRunOnce) | **POST** /scheduled_plans/run_once | Run Scheduled Plan Once
[**scheduledPlansForDashboard**](ScheduledPlanApi.md#scheduledPlansForDashboard) | **GET** /scheduled_plans/dashboard/{dashboard_id} | Scheduled Plans for Dashboard
[**scheduledPlansForLook**](ScheduledPlanApi.md#scheduledPlansForLook) | **GET** /scheduled_plans/look/{look_id} | Scheduled Plans for Look
[**scheduledPlansForLookmlDashboard**](ScheduledPlanApi.md#scheduledPlansForLookmlDashboard) | **GET** /scheduled_plans/lookml_dashboard/{lookml_dashboard_id} | Scheduled Plans for LookML Dashboard
[**scheduledPlansForSpace**](ScheduledPlanApi.md#scheduledPlansForSpace) | **GET** /scheduled_plans/space/{space_id} | Scheduled Plans for Space
[**updateScheduledPlan**](ScheduledPlanApi.md#updateScheduledPlan) | **PATCH** /scheduled_plans/{scheduled_plan_id} | Update Scheduled Plan


# **allScheduledPlans**
> \Swagger\Client\Model\ScheduledPlan[] allScheduledPlans($user_id, $fields)

Get All Scheduled Plans

### List all scheduled plans which belong to the requesting user

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | User Id (default is requesting user if not specified)
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allScheduledPlans($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->allScheduledPlans: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| User Id (default is requesting user if not specified) | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan[]**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createScheduledPlan**
> \Swagger\Client\Model\ScheduledPlan createScheduledPlan($body)

Create Scheduled Plan

### Schedule a Look or Dashboard by creating a scheduled plan.  Admins can create scheduled plans on behalf of other users by specifying a user id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\ScheduledPlan(); // \Swagger\Client\Model\ScheduledPlan | Scheduled Plan

try {
    $result = $apiInstance->createScheduledPlan($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->createScheduledPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)| Scheduled Plan | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteScheduledPlan**
> string deleteScheduledPlan($scheduled_plan_id)

Delete Scheduled Plan

### Delete the scheduled plan with the specified id.  Admins can delete other users' Scheduled Plans.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$scheduled_plan_id = 789; // int | Scheduled Plan Id

try {
    $result = $apiInstance->deleteScheduledPlan($scheduled_plan_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->deleteScheduledPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scheduled_plan_id** | **int**| Scheduled Plan Id |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **scheduledPlan**
> \Swagger\Client\Model\ScheduledPlan scheduledPlan($scheduled_plan_id, $fields)

Get Scheduled Plan

### Get information about a scheduled plan.  Admins can fetch information about other users' Scheduled Plans.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$scheduled_plan_id = 789; // int | Scheduled Plan Id
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->scheduledPlan($scheduled_plan_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->scheduledPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scheduled_plan_id** | **int**| Scheduled Plan Id |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **scheduledPlanRunOnce**
> \Swagger\Client\Model\ScheduledPlan scheduledPlanRunOnce($body)

Run Scheduled Plan Once

### Schedule a Look or Dashboard to run once _now_ with a scheduled plan.  This can be useful for testing a Scheduled Plan before committing to a production schedule.  Admins can create scheduled plans on behalf of other users by specifying a user id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Model\ScheduledPlan(); // \Swagger\Client\Model\ScheduledPlan | Scheduled Plan

try {
    $result = $apiInstance->scheduledPlanRunOnce($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->scheduledPlanRunOnce: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)| Scheduled Plan | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **scheduledPlansForDashboard**
> \Swagger\Client\Model\ScheduledPlan[] scheduledPlansForDashboard($dashboard_id, $user_id, $fields)

Scheduled Plans for Dashboard

### Get scheduled plans by using a dashboard id for the requesting user or a specified user id (with :see_schedules permission)

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$dashboard_id = 789; // int | Dashboard Id
$user_id = 789; // int | User Id (default is requesting user if not specified)
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->scheduledPlansForDashboard($dashboard_id, $user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->scheduledPlansForDashboard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dashboard_id** | **int**| Dashboard Id |
 **user_id** | **int**| User Id (default is requesting user if not specified) | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan[]**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **scheduledPlansForLook**
> \Swagger\Client\Model\ScheduledPlan[] scheduledPlansForLook($look_id, $user_id, $fields)

Scheduled Plans for Look

### Get scheduled plans by using a look id for the requesting user or a specified user id (with :see_schedules permission)

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$look_id = 789; // int | Look Id
$user_id = 789; // int | User Id (default is requesting user if not specified)
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->scheduledPlansForLook($look_id, $user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->scheduledPlansForLook: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **look_id** | **int**| Look Id |
 **user_id** | **int**| User Id (default is requesting user if not specified) | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan[]**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **scheduledPlansForLookmlDashboard**
> \Swagger\Client\Model\ScheduledPlan[] scheduledPlansForLookmlDashboard($lookml_dashboard_id, $user_id, $fields)

Scheduled Plans for LookML Dashboard

### Get scheduled plans by using a LookML dashboard id for the requesting user or a specified user id (with :see_schedules permission)

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$lookml_dashboard_id = 789; // int | LookML Dashboard Id
$user_id = 789; // int | User Id (default is requesting user if not specified)
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->scheduledPlansForLookmlDashboard($lookml_dashboard_id, $user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->scheduledPlansForLookmlDashboard: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lookml_dashboard_id** | **int**| LookML Dashboard Id |
 **user_id** | **int**| User Id (default is requesting user if not specified) | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan[]**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **scheduledPlansForSpace**
> \Swagger\Client\Model\ScheduledPlan[] scheduledPlansForSpace($space_id, $fields)

Scheduled Plans for Space

### Get scheduled plans by using a space id for the requesting user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$space_id = 789; // int | Space Id
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->scheduledPlansForSpace($space_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->scheduledPlansForSpace: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **space_id** | **int**| Space Id |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Model\ScheduledPlan[]**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateScheduledPlan**
> \Swagger\Client\Model\ScheduledPlan updateScheduledPlan($scheduled_plan_id, $body)

Update Scheduled Plan

### Update the scheduled plan with the specified id.  Admins can update other users' Scheduled Plans.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ScheduledPlanApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$scheduled_plan_id = 789; // int | Scheduled Plan Id
$body = new \Swagger\Client\Model\ScheduledPlan(); // \Swagger\Client\Model\ScheduledPlan | Scheduled Plan

try {
    $result = $apiInstance->updateScheduledPlan($scheduled_plan_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ScheduledPlanApi->updateScheduledPlan: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **scheduled_plan_id** | **int**| Scheduled Plan Id |
 **body** | [**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)| Scheduled Plan |

### Return type

[**\Swagger\Client\Model\ScheduledPlan**](../Model/ScheduledPlan.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


# Looker\UserAttributeApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allUserAttributeGroupValues**](UserAttributeApi.md#allUserAttributeGroupValues) | **GET** /user_attributes/{user_attribute_id}/group_values | Get User Attribute Group Values
[**allUserAttributes**](UserAttributeApi.md#allUserAttributes) | **GET** /user_attributes | Get All User Attributes
[**createUserAttribute**](UserAttributeApi.md#createUserAttribute) | **POST** /user_attributes | Create User Attribute
[**deleteUserAttribute**](UserAttributeApi.md#deleteUserAttribute) | **DELETE** /user_attributes/{user_attribute_id} | Delete User Attribute
[**setUserAttributeGroupValues**](UserAttributeApi.md#setUserAttributeGroupValues) | **POST** /user_attributes/{user_attribute_id}/group_values | Set User Attribute Group Values
[**updateUserAttribute**](UserAttributeApi.md#updateUserAttribute) | **PATCH** /user_attributes/{user_attribute_id} | Update User Attribute
[**userAttribute**](UserAttributeApi.md#userAttribute) | **GET** /user_attributes/{user_attribute_id} | Get User Attribute


# **allUserAttributeGroupValues**
> \Looker\Model\UserAttributeGroupValue[] allUserAttributeGroupValues($user_attribute_id, $fields)

Get User Attribute Group Values

### Returns all values of a user attribute defined by user groups, in precedence order.  A user may be a member of multiple groups which define different values for a given user attribute. The order of group-values in the response determines precedence for selecting which group-value applies to a given user.  For more information, see [Set User Attribute Group Values](#!/UserAttribute/set_user_attribute_group_values).  Results will only include groups that the caller's user account has permission to see.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_attribute_id = 789; // int | Id of user attribute
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allUserAttributeGroupValues($user_attribute_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->allUserAttributeGroupValues: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_attribute_id** | **int**| Id of user attribute |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\UserAttributeGroupValue[]**](../Model/UserAttributeGroupValue.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allUserAttributes**
> \Looker\Model\UserAttribute[] allUserAttributes($fields, $sorts)

Get All User Attributes

### Get information about all user attributes.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$sorts = "sorts_example"; // string | Fields to sort by.

try {
    $result = $apiInstance->allUserAttributes($fields, $sorts);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->allUserAttributes: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]

### Return type

[**\Looker\Model\UserAttribute[]**](../Model/UserAttribute.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserAttribute**
> \Looker\Model\UserAttribute createUserAttribute($body, $fields)

Create User Attribute

### Create a new user attribute.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Looker\Model\UserAttribute(); // \Looker\Model\UserAttribute | User Attribute
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUserAttribute($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->createUserAttribute: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Looker\Model\UserAttribute**](../Model/UserAttribute.md)| User Attribute | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\UserAttribute**](../Model/UserAttribute.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserAttribute**
> string deleteUserAttribute($user_attribute_id)

Delete User Attribute

### Delete a user attribute (admin only).

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_attribute_id = 789; // int | Id of user_attribute

try {
    $result = $apiInstance->deleteUserAttribute($user_attribute_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->deleteUserAttribute: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_attribute_id** | **int**| Id of user_attribute |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **setUserAttributeGroupValues**
> \Looker\Model\UserAttributeGroupValue[] setUserAttributeGroupValues($user_attribute_id, $body)

Set User Attribute Group Values

### Define values for a user attribute across a set of groups, in priority order.  This function defines all values for a user attribute defined by user groups. This is a global setting, potentially affecting all users in the system. This function replaces any existing group value definitions for the indicated user attribute.  The value of a user attribute for a given user is determined by searching the following locations, in this order:  1. the user's account settings 2. the groups that the user is a member of 3. the default value of the user attribute, if any  The user may be a member of multiple groups which define different values for that user attribute. The order of items in the group_values parameter determines which group takes priority for that user. Lowest array index wins.  An alternate method to indicate the selection precedence of group-values is to assign numbers to the 'rank' property of each group-value object in the array. Lowest 'rank' value wins. If you use this technique, you must assign a rank value to every group-value object in the array.  To set a user attribute value for a single user, see [Set User Attribute User Value](#!/User/set_user_attribute_user_value). To set a user attribute value for all members of a group, see [Set User Attribute Group Value](#!/Group/update_user_attribute_group_value).

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_attribute_id = 789; // int | Id of user attribute
$body = array(new \Looker\Model\UserAttributeGroupValue()); // \Looker\Model\UserAttributeGroupValue[] | Array of group values.

try {
    $result = $apiInstance->setUserAttributeGroupValues($user_attribute_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->setUserAttributeGroupValues: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_attribute_id** | **int**| Id of user attribute |
 **body** | [**\Looker\Model\UserAttributeGroupValue[]**](../Model/UserAttributeGroupValue.md)| Array of group values. |

### Return type

[**\Looker\Model\UserAttributeGroupValue[]**](../Model/UserAttributeGroupValue.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateUserAttribute**
> \Looker\Model\UserAttribute updateUserAttribute($user_attribute_id, $body, $fields)

Update User Attribute

### Update a user attribute definition.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_attribute_id = 789; // int | Id of user attribute
$body = new \Looker\Model\UserAttribute(); // \Looker\Model\UserAttribute | User Attribute
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateUserAttribute($user_attribute_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->updateUserAttribute: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_attribute_id** | **int**| Id of user attribute |
 **body** | [**\Looker\Model\UserAttribute**](../Model/UserAttribute.md)| User Attribute |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\UserAttribute**](../Model/UserAttribute.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userAttribute**
> \Looker\Model\UserAttribute userAttribute($user_attribute_id, $fields)

Get User Attribute

### Get information about a user attribute.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Looker\Api\UserAttributeApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_attribute_id = 789; // int | Id of user attribute
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userAttribute($user_attribute_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserAttributeApi->userAttribute: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_attribute_id** | **int**| Id of user attribute |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Looker\Model\UserAttribute**](../Model/UserAttribute.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


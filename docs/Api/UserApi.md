# Swagger\Client\UserApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allUserAccessFilters**](UserApi.md#allUserAccessFilters) | **GET** /users/{user_id}/access_filters | Get All Access Filters
[**allUserCredentialsApi3s**](UserApi.md#allUserCredentialsApi3s) | **GET** /users/{user_id}/credentials_api3 | Get All API 3 Credentials
[**allUserCredentialsEmbeds**](UserApi.md#allUserCredentialsEmbeds) | **GET** /users/{user_id}/credentials_embed | Get All Embedding Credentials
[**allUserSessions**](UserApi.md#allUserSessions) | **GET** /users/{user_id}/sessions | Get All Web Login Sessions
[**allUsers**](UserApi.md#allUsers) | **GET** /users | Get All Users
[**createUser**](UserApi.md#createUser) | **POST** /users | Create User
[**createUserAccessFilter**](UserApi.md#createUserAccessFilter) | **POST** /users/{user_id}/access_filters | Create Access Filter
[**createUserCredentialsApi**](UserApi.md#createUserCredentialsApi) | **POST** /users/{user_id}/credentials_api | Create API Credential
[**createUserCredentialsApi3**](UserApi.md#createUserCredentialsApi3) | **POST** /users/{user_id}/credentials_api3 | Create API 3 Credential
[**createUserCredentialsEmail**](UserApi.md#createUserCredentialsEmail) | **POST** /users/{user_id}/credentials_email | Create Email/Password Credential
[**createUserCredentialsEmailPasswordReset**](UserApi.md#createUserCredentialsEmailPasswordReset) | **POST** /users/{user_id}/credentials_email/password_reset | Create Password Reset Token
[**createUserCredentialsTotp**](UserApi.md#createUserCredentialsTotp) | **POST** /users/{user_id}/credentials_totp | Create Two-Factor Credential
[**deleteUser**](UserApi.md#deleteUser) | **DELETE** /users/{user_id} | Delete User
[**deleteUserAccessFilter**](UserApi.md#deleteUserAccessFilter) | **DELETE** /users/{user_id}/access_filters/{access_filter_id} | Delete Access Filter
[**deleteUserAttributeUserValue**](UserApi.md#deleteUserAttributeUserValue) | **DELETE** /users/{user_id}/attribute_values/{user_attribute_id} | Delete User Attribute User Value
[**deleteUserCredentialsApi**](UserApi.md#deleteUserCredentialsApi) | **DELETE** /users/{user_id}/credentials_api | Delete API Credential
[**deleteUserCredentialsApi3**](UserApi.md#deleteUserCredentialsApi3) | **DELETE** /users/{user_id}/credentials_api3/{credentials_api3_id} | Delete API 3 Credential
[**deleteUserCredentialsEmail**](UserApi.md#deleteUserCredentialsEmail) | **DELETE** /users/{user_id}/credentials_email | Delete Email/Password Credential
[**deleteUserCredentialsEmbed**](UserApi.md#deleteUserCredentialsEmbed) | **DELETE** /users/{user_id}/credentials_embed/{credentials_embed_id} | Delete Embedding Credential
[**deleteUserCredentialsGoogle**](UserApi.md#deleteUserCredentialsGoogle) | **DELETE** /users/{user_id}/credentials_google | Delete Google Auth Credential
[**deleteUserCredentialsLdap**](UserApi.md#deleteUserCredentialsLdap) | **DELETE** /users/{user_id}/credentials_ldap | Delete LDAP Credential
[**deleteUserCredentialsLookerOpenid**](UserApi.md#deleteUserCredentialsLookerOpenid) | **DELETE** /users/{user_id}/credentials_looker_openid | Delete Looker OpenId Credential
[**deleteUserCredentialsOidc**](UserApi.md#deleteUserCredentialsOidc) | **DELETE** /users/{user_id}/credentials_oidc | Delete OIDC Auth Credential
[**deleteUserCredentialsSaml**](UserApi.md#deleteUserCredentialsSaml) | **DELETE** /users/{user_id}/credentials_saml | Delete Saml Auth Credential
[**deleteUserCredentialsTotp**](UserApi.md#deleteUserCredentialsTotp) | **DELETE** /users/{user_id}/credentials_totp | Delete Two-Factor Credential
[**deleteUserSession**](UserApi.md#deleteUserSession) | **DELETE** /users/{user_id}/sessions/{session_id} | Delete Web Login Session
[**me**](UserApi.md#me) | **GET** /user | Get Current User
[**searchUsers**](UserApi.md#searchUsers) | **GET** /users/search | Search Users
[**searchUsersNames**](UserApi.md#searchUsersNames) | **GET** /users/search/names/{pattern} | Search User Names
[**setUserAttributeUserValue**](UserApi.md#setUserAttributeUserValue) | **PATCH** /users/{user_id}/attribute_values/{user_attribute_id} | Set User Attribute User Value
[**setUserRoles**](UserApi.md#setUserRoles) | **PUT** /users/{user_id}/roles | Set User Roles
[**updateUser**](UserApi.md#updateUser) | **PATCH** /users/{user_id} | Update User
[**updateUserAccessFilter**](UserApi.md#updateUserAccessFilter) | **PATCH** /users/{user_id}/access_filters/{access_filter_id} | Update Access Filter
[**updateUserCredentialsEmail**](UserApi.md#updateUserCredentialsEmail) | **PATCH** /users/{user_id}/credentials_email | Update Email/Password Credential
[**user**](UserApi.md#user) | **GET** /users/{user_id} | Get User by Id
[**userAccessFilter**](UserApi.md#userAccessFilter) | **GET** /users/{user_id}/access_filters/{access_filter_id} | Get Access Filter
[**userAttributeUserValues**](UserApi.md#userAttributeUserValues) | **GET** /users/{user_id}/attribute_values | Get User Attribute Values
[**userCredentialsApi**](UserApi.md#userCredentialsApi) | **GET** /users/{user_id}/credentials_api | Get API Credential
[**userCredentialsApi3**](UserApi.md#userCredentialsApi3) | **GET** /users/{user_id}/credentials_api3/{credentials_api3_id} | Get API 3 Credential
[**userCredentialsEmail**](UserApi.md#userCredentialsEmail) | **GET** /users/{user_id}/credentials_email | Get Email/Password Credential
[**userCredentialsEmbed**](UserApi.md#userCredentialsEmbed) | **GET** /users/{user_id}/credentials_embed/{credentials_embed_id} | Get Embedding Credential
[**userCredentialsGoogle**](UserApi.md#userCredentialsGoogle) | **GET** /users/{user_id}/credentials_google | Get Google Auth Credential
[**userCredentialsLdap**](UserApi.md#userCredentialsLdap) | **GET** /users/{user_id}/credentials_ldap | Get LDAP Credential
[**userCredentialsLookerOpenid**](UserApi.md#userCredentialsLookerOpenid) | **GET** /users/{user_id}/credentials_looker_openid | Get Looker OpenId Credential
[**userCredentialsOidc**](UserApi.md#userCredentialsOidc) | **GET** /users/{user_id}/credentials_oidc | Get OIDC Auth Credential
[**userCredentialsSaml**](UserApi.md#userCredentialsSaml) | **GET** /users/{user_id}/credentials_saml | Get Saml Auth Credential
[**userCredentialsTotp**](UserApi.md#userCredentialsTotp) | **GET** /users/{user_id}/credentials_totp | Get Two-Factor Credential
[**userForCredential**](UserApi.md#userForCredential) | **GET** /users/credential/{credential_type}/{credential_id} | Get User by Credential Id
[**userRoles**](UserApi.md#userRoles) | **GET** /users/{user_id}/roles | Get User Roles
[**userSession**](UserApi.md#userSession) | **GET** /users/{user_id}/sessions/{session_id} | Get Web Login Session


# **allUserAccessFilters**
> \Swagger\Client\Looker\Model\AccessFilter[] allUserAccessFilters($user_id, $fields)

Get All Access Filters

### Access filter for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allUserAccessFilters($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->allUserAccessFilters: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\AccessFilter[]**](../Model/AccessFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allUserCredentialsApi3s**
> \Swagger\Client\Looker\Model\CredentialsApi3[] allUserCredentialsApi3s($user_id, $fields)

Get All API 3 Credentials

### API 3 login information for the specified user. This is for the newer API keys that can be added for any user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allUserCredentialsApi3s($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->allUserCredentialsApi3s: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsApi3[]**](../Model/CredentialsApi3.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allUserCredentialsEmbeds**
> \Swagger\Client\Looker\Model\CredentialsEmbed[] allUserCredentialsEmbeds($user_id, $fields)

Get All Embedding Credentials

### Embed login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allUserCredentialsEmbeds($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->allUserCredentialsEmbeds: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsEmbed[]**](../Model/CredentialsEmbed.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allUserSessions**
> \Swagger\Client\Looker\Model\Session[] allUserSessions($user_id, $fields)

Get All Web Login Sessions

### Web login session for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->allUserSessions($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->allUserSessions: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Session[]**](../Model/Session.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allUsers**
> \Swagger\Client\Looker\Model\User[] allUsers($fields, $page, $per_page, $sorts, $ids)

Get All Users

### Get information about all users.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$page = 789; // int | Requested page.
$per_page = 789; // int | Results per page.
$sorts = "sorts_example"; // string | Fields to sort by.
$ids = array(56); // int[] | Optional list of ids to get specific users.

try {
    $result = $apiInstance->allUsers($fields, $page, $per_page, $sorts, $ids);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->allUsers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **page** | **int**| Requested page. | [optional]
 **per_page** | **int**| Results per page. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **ids** | [**int[]**](../Model/int.md)| Optional list of ids to get specific users. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User[]**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUser**
> \Swagger\Client\Looker\Model\User createUser($body, $fields)

Create User

### Create a user with the specified information.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Looker\Model\User(); // \Swagger\Client\Looker\Model\User | User
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUser($body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Looker\Model\User**](../Model/User.md)| User | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserAccessFilter**
> \Swagger\Client\Looker\Model\AccessFilter createUserAccessFilter($user_id, $body, $fields)

Create Access Filter

### Access filter for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$body = new \Swagger\Client\Looker\Model\AccessFilter(); // \Swagger\Client\Looker\Model\AccessFilter | Access Filter
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUserAccessFilter($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUserAccessFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **body** | [**\Swagger\Client\Looker\Model\AccessFilter**](../Model/AccessFilter.md)| Access Filter | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\AccessFilter**](../Model/AccessFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserCredentialsApi**
> \Swagger\Client\Looker\Model\CredentialsApi createUserCredentialsApi($user_id, $body)

Create API Credential

### Create API Credential. SUPPORT FOR THIS HAS BEEN REMOVED.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$body = new \Swagger\Client\Looker\Model\CredentialsApi(); // \Swagger\Client\Looker\Model\CredentialsApi | API Credential

try {
    $result = $apiInstance->createUserCredentialsApi($user_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUserCredentialsApi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **body** | [**\Swagger\Client\Looker\Model\CredentialsApi**](../Model/CredentialsApi.md)| API Credential | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsApi**](../Model/CredentialsApi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserCredentialsApi3**
> \Swagger\Client\Looker\Model\CredentialsApi3 createUserCredentialsApi3($user_id, $body, $fields)

Create API 3 Credential

### API 3 login information for the specified user. This is for the newer API keys that can be added for any user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$body = new \Swagger\Client\Looker\Model\CredentialsApi3(); // \Swagger\Client\Looker\Model\CredentialsApi3 | API 3 Credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUserCredentialsApi3($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUserCredentialsApi3: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **body** | [**\Swagger\Client\Looker\Model\CredentialsApi3**](../Model/CredentialsApi3.md)| API 3 Credential | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsApi3**](../Model/CredentialsApi3.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserCredentialsEmail**
> \Swagger\Client\Looker\Model\CredentialsEmail createUserCredentialsEmail($user_id, $body, $fields)

Create Email/Password Credential

### Email/password login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$body = new \Swagger\Client\Looker\Model\CredentialsEmail(); // \Swagger\Client\Looker\Model\CredentialsEmail | Email/Password Credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUserCredentialsEmail($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUserCredentialsEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **body** | [**\Swagger\Client\Looker\Model\CredentialsEmail**](../Model/CredentialsEmail.md)| Email/Password Credential | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsEmail**](../Model/CredentialsEmail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserCredentialsEmailPasswordReset**
> \Swagger\Client\Looker\Model\CredentialsEmail createUserCredentialsEmailPasswordReset($user_id, $expires, $fields)

Create Password Reset Token

### Create a password reset token. This will create a cryptographically secure random password reset token for the user. If the user already has a password reset token then this invalidates the old token and creates a new one. The token is expressed as the 'password_reset_url' of the user's email/password credential object. This takes an optional 'expires' param to indicate if the new token should be an expiring token. Tokens that expire are typically used for self-service password resets for existing users. Invitation emails for new users typically are not set to expire. The expire period is always 60 minutes when expires is enabled. This method can be called with an empty body.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$expires = true; // bool | Expiring token.
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUserCredentialsEmailPasswordReset($user_id, $expires, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUserCredentialsEmailPasswordReset: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **expires** | **bool**| Expiring token. | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsEmail**](../Model/CredentialsEmail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createUserCredentialsTotp**
> \Swagger\Client\Looker\Model\CredentialsTotp createUserCredentialsTotp($user_id, $body, $fields)

Create Two-Factor Credential

### Two-factor login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$body = new \Swagger\Client\Looker\Model\CredentialsTotp(); // \Swagger\Client\Looker\Model\CredentialsTotp | Two-Factor Credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->createUserCredentialsTotp($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->createUserCredentialsTotp: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **body** | [**\Swagger\Client\Looker\Model\CredentialsTotp**](../Model/CredentialsTotp.md)| Two-Factor Credential | [optional]
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsTotp**](../Model/CredentialsTotp.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUser**
> string deleteUser($user_id)

Delete User

### Delete the user with a specific id.  **DANGER** this will delete the user and all looks and other information owned by the user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user

try {
    $result = $apiInstance->deleteUser($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserAccessFilter**
> string deleteUserAccessFilter($user_id, $access_filter_id)

Delete Access Filter

### Access filter for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$access_filter_id = 789; // int | id of Access Filter

try {
    $result = $apiInstance->deleteUserAccessFilter($user_id, $access_filter_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserAccessFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **access_filter_id** | **int**| id of Access Filter |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserAttributeUserValue**
> deleteUserAttributeUserValue($user_id, $user_attribute_id)

Delete User Attribute User Value

### Delete a user attribute value from a user's account settings.  After the user attribute value is deleted from the user's account settings, subsequent requests for the user attribute value for this user will draw from the user's groups or the default value of the user attribute. See [Get User Attribute Values](#!/User/user_attribute_user_values) for more information about how user attribute values are resolved.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$user_attribute_id = 789; // int | Id of user attribute

try {
    $apiInstance->deleteUserAttributeUserValue($user_id, $user_attribute_id);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserAttributeUserValue: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **user_attribute_id** | **int**| Id of user attribute |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsApi**
> string deleteUserCredentialsApi($user_id)

Delete API Credential

### API login information for the specified user. This is for 'API Users' used for the 'old' query API. THIS SUPPORT HAS BEEN REMOVED.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsApi($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsApi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsApi3**
> string deleteUserCredentialsApi3($user_id, $credentials_api3_id)

Delete API 3 Credential

### API 3 login information for the specified user. This is for the newer API keys that can be added for any user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$credentials_api3_id = 789; // int | id of API 3 Credential

try {
    $result = $apiInstance->deleteUserCredentialsApi3($user_id, $credentials_api3_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsApi3: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **credentials_api3_id** | **int**| id of API 3 Credential |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsEmail**
> string deleteUserCredentialsEmail($user_id)

Delete Email/Password Credential

### Email/password login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsEmail($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsEmbed**
> string deleteUserCredentialsEmbed($user_id, $credentials_embed_id)

Delete Embedding Credential

### Embed login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$credentials_embed_id = 789; // int | id of Embedding Credential

try {
    $result = $apiInstance->deleteUserCredentialsEmbed($user_id, $credentials_embed_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsEmbed: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **credentials_embed_id** | **int**| id of Embedding Credential |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsGoogle**
> string deleteUserCredentialsGoogle($user_id)

Delete Google Auth Credential

### Google authentication login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsGoogle($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsGoogle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsLdap**
> string deleteUserCredentialsLdap($user_id)

Delete LDAP Credential

### LDAP login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsLdap($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsLdap: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsLookerOpenid**
> string deleteUserCredentialsLookerOpenid($user_id)

Delete Looker OpenId Credential

### Looker Openid login information for the specified user. Used by Looker Analysts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsLookerOpenid($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsLookerOpenid: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsOidc**
> string deleteUserCredentialsOidc($user_id)

Delete OIDC Auth Credential

### OpenID Connect (OIDC) authentication login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsOidc($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsOidc: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsSaml**
> string deleteUserCredentialsSaml($user_id)

Delete Saml Auth Credential

### Saml authentication login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsSaml($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsSaml: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserCredentialsTotp**
> string deleteUserCredentialsTotp($user_id)

Delete Two-Factor Credential

### Two-factor login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user

try {
    $result = $apiInstance->deleteUserCredentialsTotp($user_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserCredentialsTotp: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteUserSession**
> string deleteUserSession($user_id, $session_id)

Delete Web Login Session

### Web login session for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$session_id = 789; // int | id of Web Login Session

try {
    $result = $apiInstance->deleteUserSession($user_id, $session_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->deleteUserSession: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **session_id** | **int**| id of Web Login Session |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **me**
> \Swagger\Client\Looker\Model\User me($fields)

Get Current User

### Get information about the current user; i.e. the user account currently calling the API.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->me($fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->me: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchUsers**
> \Swagger\Client\Looker\Model\User[] searchUsers($fields, $page, $per_page, $sorts, $id, $first_name, $last_name, $verified_looker_employee, $email, $is_disabled, $filter_or, $content_metadata_id, $group_id)

Search Users

### Search users.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields.
$page = 789; // int | Requested page.
$per_page = 789; // int | Results per page.
$sorts = "sorts_example"; // string | Fields to sort by.
$id = 789; // int | Match User Id.
$first_name = "first_name_example"; // string | Match First name.
$last_name = "last_name_example"; // string | Match Last name.
$verified_looker_employee = true; // bool | Match Verified Looker employee.
$email = "email_example"; // string | Match Email Address.
$is_disabled = true; // bool | Match Is disabled.
$filter_or = true; // bool | Do an OR search with parameters
$content_metadata_id = 789; // int | Id of content metadata to which users must have access
$group_id = 789; // int | Id of group of which users must be directly members

try {
    $result = $apiInstance->searchUsers($fields, $page, $per_page, $sorts, $id, $first_name, $last_name, $verified_looker_employee, $email, $is_disabled, $filter_or, $content_metadata_id, $group_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->searchUsers: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields. | [optional]
 **page** | **int**| Requested page. | [optional]
 **per_page** | **int**| Results per page. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **id** | **int**| Match User Id. | [optional]
 **first_name** | **string**| Match First name. | [optional]
 **last_name** | **string**| Match Last name. | [optional]
 **verified_looker_employee** | **bool**| Match Verified Looker employee. | [optional]
 **email** | **string**| Match Email Address. | [optional]
 **is_disabled** | **bool**| Match Is disabled. | [optional]
 **filter_or** | **bool**| Do an OR search with parameters | [optional]
 **content_metadata_id** | **int**| Id of content metadata to which users must have access | [optional]
 **group_id** | **int**| Id of group of which users must be directly members | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User[]**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchUsersNames**
> \Swagger\Client\Looker\Model\User[] searchUsersNames($pattern, $fields, $page, $per_page, $sorts, $id, $first_name, $last_name, $verified_looker_employee, $email, $is_disabled)

Search User Names

### Search users where first_name OR last_name OR email matches a string.  The results will be AND'd with any additional search parameters that are (optionally) included.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$pattern = "pattern_example"; // string | Pattern to match.
$fields = "fields_example"; // string | Requested fields.
$page = 789; // int | Requested page.
$per_page = 789; // int | Results per page.
$sorts = "sorts_example"; // string | Fields to sort by.
$id = 789; // int | Match User Id.
$first_name = "first_name_example"; // string | Match First name.
$last_name = "last_name_example"; // string | Match Last name.
$verified_looker_employee = true; // bool | Match Verified Looker employee.
$email = "email_example"; // string | Match Email Address.
$is_disabled = true; // bool | Match Is disabled.

try {
    $result = $apiInstance->searchUsersNames($pattern, $fields, $page, $per_page, $sorts, $id, $first_name, $last_name, $verified_looker_employee, $email, $is_disabled);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->searchUsersNames: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **pattern** | **string**| Pattern to match. |
 **fields** | **string**| Requested fields. | [optional]
 **page** | **int**| Requested page. | [optional]
 **per_page** | **int**| Results per page. | [optional]
 **sorts** | **string**| Fields to sort by. | [optional]
 **id** | **int**| Match User Id. | [optional]
 **first_name** | **string**| Match First name. | [optional]
 **last_name** | **string**| Match Last name. | [optional]
 **verified_looker_employee** | **bool**| Match Verified Looker employee. | [optional]
 **email** | **string**| Match Email Address. | [optional]
 **is_disabled** | **bool**| Match Is disabled. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User[]**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **setUserAttributeUserValue**
> \Swagger\Client\Looker\Model\UserAttributeWithValue setUserAttributeUserValue($user_id, $user_attribute_id, $body)

Set User Attribute User Value

### Store a custom value for a user attribute in a user's account settings.  Per-user user attribute values take precedence over group or default values.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$user_attribute_id = 789; // int | Id of user attribute
$body = new \Swagger\Client\Looker\Model\UserAttributeWithValue(); // \Swagger\Client\Looker\Model\UserAttributeWithValue | New attribute value for user.

try {
    $result = $apiInstance->setUserAttributeUserValue($user_id, $user_attribute_id, $body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->setUserAttributeUserValue: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **user_attribute_id** | **int**| Id of user attribute |
 **body** | [**\Swagger\Client\Looker\Model\UserAttributeWithValue**](../Model/UserAttributeWithValue.md)| New attribute value for user. |

### Return type

[**\Swagger\Client\Looker\Model\UserAttributeWithValue**](../Model/UserAttributeWithValue.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **setUserRoles**
> \Swagger\Client\Looker\Model\Role[] setUserRoles($user_id, $body, $fields)

Set User Roles

### Set roles of the user with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$body = array(new \Swagger\Client\Looker\Model\int[]()); // int[] | array of roles ids for user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->setUserRoles($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->setUserRoles: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **body** | **int[]**| array of roles ids for user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Role[]**](../Model/Role.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateUser**
> \Swagger\Client\Looker\Model\User updateUser($user_id, $body, $fields)

Update User

### Update information about the user with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$body = new \Swagger\Client\Looker\Model\User(); // \Swagger\Client\Looker\Model\User | User
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateUser($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->updateUser: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **body** | [**\Swagger\Client\Looker\Model\User**](../Model/User.md)| User |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateUserAccessFilter**
> \Swagger\Client\Looker\Model\AccessFilter updateUserAccessFilter($user_id, $access_filter_id, $body, $fields)

Update Access Filter

### Access filter for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$access_filter_id = 789; // int | id of Access Filter
$body = new \Swagger\Client\Looker\Model\AccessFilter(); // \Swagger\Client\Looker\Model\AccessFilter | Access Filter
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateUserAccessFilter($user_id, $access_filter_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->updateUserAccessFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **access_filter_id** | **int**| id of Access Filter |
 **body** | [**\Swagger\Client\Looker\Model\AccessFilter**](../Model/AccessFilter.md)| Access Filter |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\AccessFilter**](../Model/AccessFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateUserCredentialsEmail**
> \Swagger\Client\Looker\Model\CredentialsEmail updateUserCredentialsEmail($user_id, $body, $fields)

Update Email/Password Credential

### Email/password login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$body = new \Swagger\Client\Looker\Model\CredentialsEmail(); // \Swagger\Client\Looker\Model\CredentialsEmail | Email/Password Credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->updateUserCredentialsEmail($user_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->updateUserCredentialsEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **body** | [**\Swagger\Client\Looker\Model\CredentialsEmail**](../Model/CredentialsEmail.md)| Email/Password Credential |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsEmail**](../Model/CredentialsEmail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **user**
> \Swagger\Client\Looker\Model\User user($user_id, $fields)

Get User by Id

### Get information about the user with a specific id.  If the caller is an admin or the caller is the user being specified, then full user information will be returned. Otherwise, a minimal 'public' variant of the user information will be returned. This contains The user name and avatar url, but no sensitive information.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->user($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->user: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userAccessFilter**
> \Swagger\Client\Looker\Model\AccessFilter userAccessFilter($user_id, $access_filter_id, $fields)

Get Access Filter

### Access filter for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$access_filter_id = 789; // int | Id of Access Filter
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userAccessFilter($user_id, $access_filter_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userAccessFilter: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **access_filter_id** | **int**| Id of Access Filter |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\AccessFilter**](../Model/AccessFilter.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userAttributeUserValues**
> \Swagger\Client\Looker\Model\UserAttributeWithValue[] userAttributeUserValues($user_id, $fields, $user_attribute_ids, $all_values, $include_unset)

Get User Attribute Values

### Get user attribute values for a given user.  Returns the values of specified user attributes (or all user attributes) for a certain user.  A value for each user attribute is searched for in the following locations, in this order: 1. in the user's account information 1. in groups that the user is a member of 1. the default value of the user attribute  If more than one group has a value defined for a user attribute, the group with the lowest rank wins.  The response will only include user attributes for which values were found. Use `include_unset=true` to include empty records for user attributes with no value.  The value of all hidden user attributes will be blank.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$fields = "fields_example"; // string | Requested fields.
$user_attribute_ids = array(56); // int[] | Specific user attributes to request. Omit or leave blank to request all user attributes.
$all_values = true; // bool | If true, returns all values in the search path instead of just the first value found. Useful for debugging group precedence.
$include_unset = true; // bool | If true, returns an empty record for each requested attribute that has no user, group, or default value.

try {
    $result = $apiInstance->userAttributeUserValues($user_id, $fields, $user_attribute_ids, $all_values, $include_unset);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userAttributeUserValues: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **fields** | **string**| Requested fields. | [optional]
 **user_attribute_ids** | [**int[]**](../Model/int.md)| Specific user attributes to request. Omit or leave blank to request all user attributes. | [optional]
 **all_values** | **bool**| If true, returns all values in the search path instead of just the first value found. Useful for debugging group precedence. | [optional]
 **include_unset** | **bool**| If true, returns an empty record for each requested attribute that has no user, group, or default value. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\UserAttributeWithValue[]**](../Model/UserAttributeWithValue.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsApi**
> \Swagger\Client\Looker\Model\CredentialsApi userCredentialsApi($user_id, $fields)

Get API Credential

### API login information for the specified user. This is for 'API Users' used for the 'old' query API. THIS SUPPORT HAS BEEN REMOVED.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsApi($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsApi: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsApi**](../Model/CredentialsApi.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsApi3**
> \Swagger\Client\Looker\Model\CredentialsApi3 userCredentialsApi3($user_id, $credentials_api3_id, $fields)

Get API 3 Credential

### API 3 login information for the specified user. This is for the newer API keys that can be added for any user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$credentials_api3_id = 789; // int | Id of API 3 Credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsApi3($user_id, $credentials_api3_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsApi3: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **credentials_api3_id** | **int**| Id of API 3 Credential |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsApi3**](../Model/CredentialsApi3.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsEmail**
> \Swagger\Client\Looker\Model\CredentialsEmail userCredentialsEmail($user_id, $fields)

Get Email/Password Credential

### Email/password login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsEmail($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsEmail: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsEmail**](../Model/CredentialsEmail.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsEmbed**
> \Swagger\Client\Looker\Model\CredentialsEmbed userCredentialsEmbed($user_id, $credentials_embed_id, $fields)

Get Embedding Credential

### Embed login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$credentials_embed_id = 789; // int | Id of Embedding Credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsEmbed($user_id, $credentials_embed_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsEmbed: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **credentials_embed_id** | **int**| Id of Embedding Credential |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsEmbed**](../Model/CredentialsEmbed.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsGoogle**
> \Swagger\Client\Looker\Model\CredentialsGoogle userCredentialsGoogle($user_id, $fields)

Get Google Auth Credential

### Google authentication login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsGoogle($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsGoogle: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsGoogle**](../Model/CredentialsGoogle.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsLdap**
> \Swagger\Client\Looker\Model\CredentialsLDAP userCredentialsLdap($user_id, $fields)

Get LDAP Credential

### LDAP login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsLdap($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsLdap: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsLDAP**](../Model/CredentialsLDAP.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsLookerOpenid**
> \Swagger\Client\Looker\Model\CredentialsLookerOpenid userCredentialsLookerOpenid($user_id, $fields)

Get Looker OpenId Credential

### Looker Openid login information for the specified user. Used by Looker Analysts.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsLookerOpenid($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsLookerOpenid: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsLookerOpenid**](../Model/CredentialsLookerOpenid.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsOidc**
> \Swagger\Client\Looker\Model\CredentialsOIDC userCredentialsOidc($user_id, $fields)

Get OIDC Auth Credential

### OpenID Connect (OIDC) authentication login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsOidc($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsOidc: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsOIDC**](../Model/CredentialsOIDC.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsSaml**
> \Swagger\Client\Looker\Model\CredentialsSaml userCredentialsSaml($user_id, $fields)

Get Saml Auth Credential

### Saml authentication login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsSaml($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsSaml: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsSaml**](../Model/CredentialsSaml.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userCredentialsTotp**
> \Swagger\Client\Looker\Model\CredentialsTotp userCredentialsTotp($user_id, $fields)

Get Two-Factor Credential

### Two-factor login information for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userCredentialsTotp($user_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userCredentialsTotp: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\CredentialsTotp**](../Model/CredentialsTotp.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userForCredential**
> \Swagger\Client\Looker\Model\User userForCredential($credential_type, $credential_id, $fields)

Get User by Credential Id

### Get information about the user with a credential of given type with specific id.  This is used to do things like find users by their embed external_user_id. Or, find the user with a given api3 client_id, etc. The 'credential_type' matchs the 'type' name of the various credential types. It must be one of the values listed in the table below. The 'credential_id' is your unique Id for the user and is specific to each type of credential.  An example using the Ruby sdk might look like:  `sdk.user_for_credential('embed', 'customer-4959425')`  This table shows the supported 'Credential Type' strings. The right column is for reference; it shows which field in the given credential type is actually searched when finding a user with the supplied 'credential_id'.  | Credential Types | Id Field Matched | | ---------------- | ---------------- | | email            | email            | | google           | google_user_id   | | saml             | saml_user_id     | | oidc             | oidc_user_id     | | ldap             | ldap_id          | | api              | token            | | api3             | client_id        | | embed            | external_user_id | | looker_openid    | email            |  NOTE: 'api' is the legacy Looker query API. The API you are currently looking at is 'api3'.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$credential_type = "credential_type_example"; // string | Type name of credential
$credential_id = "credential_id_example"; // string | Id of credential
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userForCredential($credential_type, $credential_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userForCredential: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **credential_type** | **string**| Type name of credential |
 **credential_id** | **string**| Id of credential |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\User**](../Model/User.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userRoles**
> \Swagger\Client\Looker\Model\Role[] userRoles($user_id, $fields, $direct_association_only)

Get User Roles

### Get information about roles of the user with a specific id.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | id of user
$fields = "fields_example"; // string | Requested fields.
$direct_association_only = true; // bool | Get only roles associated directly with the user: exclude those only associated through groups.

try {
    $result = $apiInstance->userRoles($user_id, $fields, $direct_association_only);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userRoles: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| id of user |
 **fields** | **string**| Requested fields. | [optional]
 **direct_association_only** | **bool**| Get only roles associated directly with the user: exclude those only associated through groups. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Role[]**](../Model/Role.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **userSession**
> \Swagger\Client\Looker\Model\Session userSession($user_id, $session_id, $fields)

Get Web Login Session

### Web login session for the specified user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\UserApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$user_id = 789; // int | Id of user
$session_id = 789; // int | Id of Web Login Session
$fields = "fields_example"; // string | Requested fields.

try {
    $result = $apiInstance->userSession($user_id, $session_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling UserApi->userSession: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_id** | **int**| Id of user |
 **session_id** | **int**| Id of Web Login Session |
 **fields** | **string**| Requested fields. | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Session**](../Model/Session.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


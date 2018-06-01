# Swagger\Client\ProjectApi

All URIs are relative to *https://ethosce.looker.com:19999/api/3.1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allGitBranches**](ProjectApi.md#allGitBranches) | **GET** /projects/{project_id}/git_branches | Get All Git Branchs
[**allGitConnectionTests**](ProjectApi.md#allGitConnectionTests) | **GET** /projects/{project_id}/git_connection_tests | Get All Git Connection Tests
[**allProjectFiles**](ProjectApi.md#allProjectFiles) | **GET** /projects/{project_id}/files | Get All Project Files
[**allProjects**](ProjectApi.md#allProjects) | **GET** /projects | Get All Projects
[**createGitDeployKey**](ProjectApi.md#createGitDeployKey) | **POST** /projects/{project_id}/git/deploy_key | Create Deploy Key
[**createProject**](ProjectApi.md#createProject) | **POST** /projects | Create Project
[**gitDeployKey**](ProjectApi.md#gitDeployKey) | **GET** /projects/{project_id}/git/deploy_key | Git Deploy Key
[**project**](ProjectApi.md#project) | **GET** /projects/{project_id} | Get Project
[**projectFile**](ProjectApi.md#projectFile) | **GET** /projects/{project_id}/files/file | Get Project File
[**projectValidationResults**](ProjectApi.md#projectValidationResults) | **GET** /projects/{project_id}/validate | Cached Project Validation Results
[**projectWorkspace**](ProjectApi.md#projectWorkspace) | **GET** /projects/{project_id}/current_workspace | Get Project Workspace
[**resetProjectToProduction**](ProjectApi.md#resetProjectToProduction) | **POST** /projects/{project_id}/reset_to_production | Reset To Production
[**resetProjectToRemote**](ProjectApi.md#resetProjectToRemote) | **POST** /projects/{project_id}/reset_to_remote | Reset To Remote
[**runGitConnectionTest**](ProjectApi.md#runGitConnectionTest) | **GET** /projects/{project_id}/git_connection_tests/{test_id} | Run Git Connection Test
[**updateProject**](ProjectApi.md#updateProject) | **PATCH** /projects/{project_id} | Update Project
[**validateProject**](ProjectApi.md#validateProject) | **POST** /projects/{project_id}/validate | Validate Project


# **allGitBranches**
> \Swagger\Client\Looker\Model\GitBranch[] allGitBranches($project_id)

Get All Git Branchs

### Get All Git Branches  Returns a list of git branches in the project repository

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id

try {
    $result = $apiInstance->allGitBranches($project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->allGitBranches: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |

### Return type

[**\Swagger\Client\Looker\Model\GitBranch[]**](../Model/GitBranch.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allGitConnectionTests**
> \Swagger\Client\Looker\Model\GitConnectionTest[] allGitConnectionTests($project_id)

Get All Git Connection Tests

### Get All Git Connection Tests  Returns a list of tests which can be run against a project's git connection

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id

try {
    $result = $apiInstance->allGitConnectionTests($project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->allGitConnectionTests: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |

### Return type

[**\Swagger\Client\Looker\Model\GitConnectionTest[]**](../Model/GitConnectionTest.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allProjectFiles**
> \Swagger\Client\Looker\Model\ProjectFile[] allProjectFiles($project_id, $fields)

Get All Project Files

### Get All Project Files  Returns a list of the files in the project

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->allProjectFiles($project_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->allProjectFiles: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\ProjectFile[]**](../Model/ProjectFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **allProjects**
> \Swagger\Client\Looker\Model\Project[] allProjects($fields)

Get All Projects

### Get All Projects  Returns all projects visible to the current user

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->allProjects($fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->allProjects: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Project[]**](../Model/Project.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createGitDeployKey**
> string createGitDeployKey($project_id)

Create Deploy Key

### Create Git Deploy Key  Create a public/private key pair for authenticating ssh git requests from Looker to a remote git repository for a particular Looker project.  Returns the public key of the generated ssh key pair.  Copy this public key to your remote git repository's ssh keys configuration so that the remote git service can validate and accept git requests from the Looker server.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id

try {
    $result = $apiInstance->createGitDeployKey($project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->createGitDeployKey: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text/plain

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **createProject**
> \Swagger\Client\Looker\Model\Project createProject($body)

Create Project

### Create A Project  dev mode required. - Call `update_session` to select the 'dev' workspace.  `name` is required. `git_remote_url` is not allowed. To configure Git for the newly created project, follow the instructions in `update_project`.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$body = new \Swagger\Client\Looker\Model\Project(); // \Swagger\Client\Looker\Model\Project | Project

try {
    $result = $apiInstance->createProject($body);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->createProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**\Swagger\Client\Looker\Model\Project**](../Model/Project.md)| Project | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Project**](../Model/Project.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **gitDeployKey**
> string gitDeployKey($project_id)

Git Deploy Key

### Git Deploy Key  Returns the ssh public key previously created for a project's git repository.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id

try {
    $result = $apiInstance->gitDeployKey($project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->gitDeployKey: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: text/plain

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **project**
> \Swagger\Client\Looker\Model\Project project($project_id, $fields)

Get Project

### Get A Project  Returns the project with the given project id

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->project($project_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->project: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Project**](../Model/Project.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **projectFile**
> \Swagger\Client\Looker\Model\ProjectFile projectFile($project_id, $file_id, $fields)

Get Project File

### Get Project File Info  Returns information about a file in the project

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$file_id = "file_id_example"; // string | File Id
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->projectFile($project_id, $file_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->projectFile: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **file_id** | **string**| File Id |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\ProjectFile**](../Model/ProjectFile.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **projectValidationResults**
> \Swagger\Client\Looker\Model\ProjectValidationCache projectValidationResults($project_id, $fields)

Cached Project Validation Results

### Get Cached Project Validation Results  Returns the cached results of a previous project validation calculation, if any. Returns http status 204 No Content if no validation results exist.  Validating the content of all the files in a project can be computationally intensive for large projects. Use this API to simply fetch the results of the most recent project validation rather than revalidating the entire project from scratch.  A value of `\"stale\": true` in the response indicates that the project has changed since the cached validation results were computed. The cached validation results may no longer reflect the current state of the project.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->projectValidationResults($project_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->projectValidationResults: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\ProjectValidationCache**](../Model/ProjectValidationCache.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **projectWorkspace**
> \Swagger\Client\Looker\Model\ProjectWorkspace projectWorkspace($project_id, $fields)

Get Project Workspace

### Get Project Workspace  Returns information about the state of the project files in the currently selected workspace

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->projectWorkspace($project_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->projectWorkspace: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\ProjectWorkspace**](../Model/ProjectWorkspace.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **resetProjectToProduction**
> string resetProjectToProduction($project_id)

Reset To Production

### Reset a project to the revision of the project that is in production.  **DANGER** this will delete any changes that have not been pushed to a remote repository.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Id of project

try {
    $result = $apiInstance->resetProjectToProduction($project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->resetProjectToProduction: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Id of project |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **resetProjectToRemote**
> string resetProjectToRemote($project_id)

Reset To Remote

### Reset a project development branch to the revision of the project that is on the remote.  **DANGER** this will delete any changes that have not been pushed to a remote repository.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Id of project

try {
    $result = $apiInstance->resetProjectToRemote($project_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->resetProjectToRemote: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Id of project |

### Return type

**string**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **runGitConnectionTest**
> \Swagger\Client\Looker\Model\GitConnectionTestResult runGitConnectionTest($project_id, $test_id)

Run Git Connection Test

### Run a git connection test  Run the named test on the git service used by this project and return the result. This is intended to help debug git connections when things do not work properly, to give more helpful information about why a git url is not working with Looker. They are intended to be run in the order they are returned from the /projects/ID/git_connection_tests endpoint.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$test_id = "test_id_example"; // string | Test Id

try {
    $result = $apiInstance->runGitConnectionTest($project_id, $test_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->runGitConnectionTest: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **test_id** | **string**| Test Id |

### Return type

[**\Swagger\Client\Looker\Model\GitConnectionTestResult**](../Model/GitConnectionTestResult.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **updateProject**
> \Swagger\Client\Looker\Model\Project updateProject($project_id, $body, $fields)

Update Project

### Update Project Configuration  Apply changes to a project's configuration.   #### Configuring Git for a Project  To set up a Looker project with a remote git repository, follow these steps:  1. Call `update_session` to select the 'dev' workspace. 1. Call `create_git_deploy_key` to create a new deploy key for the project 1. Copy the deploy key text into the remote git repository's ssh key configuration 1. Call `update_project` to set project's `git_remote_url` ()and `git_service_name`, if necessary).  When you modify a project's `git_remote_url`, Looker connects to the remote repository to fetch metadata. The remote git repository MUST be configured with the Looker-generated deploy key for this project prior to setting the project's `git_remote_url`.  To set up a Looker project with a git repository residing on the Looker server (a 'bare' git repo): 1. Call `update_session` to select the 'dev' workspace. 1. Call `update_project` setting `git_remote_url` to nil and `git_service_name` to \"bare\".

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$body = new \Swagger\Client\Looker\Model\Project(); // \Swagger\Client\Looker\Model\Project | Project
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->updateProject($project_id, $body, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->updateProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **body** | [**\Swagger\Client\Looker\Model\Project**](../Model/Project.md)| Project |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\Project**](../Model/Project.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **validateProject**
> \Swagger\Client\Looker\Model\ProjectValidation validateProject($project_id, $fields)

Validate Project

### Validate Project  Performs lint validation of all lookml files in the project. Returns a list of errors found, if any.  Validating the content of all the files in a project can be computationally intensive for large projects. For best performance, call `validate_project(project_id)` only when you really want to recompute project validation. To quickly display the results of the most recent project validation (without recomputing), use `project_validation_results(project_id)`

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$apiInstance = new Swagger\Client\Api\ProjectApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client()
);
$project_id = "project_id_example"; // string | Project Id
$fields = "fields_example"; // string | Requested fields

try {
    $result = $apiInstance->validateProject($project_id, $fields);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProjectApi->validateProject: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **project_id** | **string**| Project Id |
 **fields** | **string**| Requested fields | [optional]

### Return type

[**\Swagger\Client\Looker\Model\ProjectValidation**](../Model/ProjectValidation.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


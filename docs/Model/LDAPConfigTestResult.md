# LDAPConfigTestResult

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**status** | **string** | Test status code: always &#39;success&#39; or &#39;error&#39; | [optional] 
**message** | **string** | Short human readable test about the result | [optional] 
**details** | **string** | Additional details for error cases | [optional] 
**user** | [**\Swagger\Client\Model\LDAPUser**](LDAPUser.md) | User details from LDAP server for auth tests | [optional] 
**trace** | **string** | A more detailed trace incremental results during auth tests | [optional] 
**url** | **string** | Link to ldap config | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



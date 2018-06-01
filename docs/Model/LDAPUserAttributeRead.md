# LDAPUserAttributeRead

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | Name of User Attribute in LDAP | [optional] 
**required** | **bool** | Required to be in LDAP assertion for login to be allowed to succeed | [optional] 
**user_attributes** | [**\Swagger\Client\Looker\Model\UserAttribute[]**](UserAttribute.md) | Looker User Attributes | [optional] 
**url** | **string** | Link to LDAP config | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



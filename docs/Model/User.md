# User

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique Id | [optional] 
**first_name** | **string** | First name | [optional] 
**last_name** | **string** | Last name | [optional] 
**display_name** | **string** | Full name for display (available only if both first_name and last_name are set) | [optional] 
**email** | **string** | EMail address | [optional] 
**is_disabled** | **bool** | Account has been disabled | [optional] 
**avatar_url** | **string** | URL for the avatar image (may be generic) | [optional] 
**home_space_id** | **string** | ID string for user&#39;s home space | [optional] 
**personal_space_id** | **int** | ID of user&#39;s personal space | [optional] 
**embed_group_space_id** | **int** | (Embed only) ID of user&#39;s group space based on the external_group_id optionally specified during embed user login | [optional] 
**access_filters** | [**\Swagger\Client\Looker\Model\AccessFilter[]**](AccessFilter.md) | Model access filters. | [optional] 
**credentials_email** | [**\Swagger\Client\Looker\Model\CredentialsEmail**](CredentialsEmail.md) | Email/Password login credentials | [optional] 
**credentials_totp** | [**\Swagger\Client\Looker\Model\CredentialsTotp**](CredentialsTotp.md) | Two-factor credentials | [optional] 
**credentials_ldap** | [**\Swagger\Client\Looker\Model\CredentialsLDAP**](CredentialsLDAP.md) | LDAP credentials | [optional] 
**credentials_google** | [**\Swagger\Client\Looker\Model\CredentialsGoogle**](CredentialsGoogle.md) | Google auth credentials | [optional] 
**credentials_saml** | [**\Swagger\Client\Looker\Model\CredentialsSaml**](CredentialsSaml.md) | Saml auth credentials | [optional] 
**credentials_oidc** | [**\Swagger\Client\Looker\Model\CredentialsOIDC**](CredentialsOIDC.md) | OpenID Connect auth credentials | [optional] 
**credentials_api** | [**\Swagger\Client\Looker\Model\CredentialsApi**](CredentialsApi.md) | API user credentials. NO LONGER SUPPORTED. | [optional] 
**credentials_api3** | [**\Swagger\Client\Looker\Model\CredentialsApi3[]**](CredentialsApi3.md) | API 3 credentials | [optional] 
**credentials_embed** | [**\Swagger\Client\Looker\Model\CredentialsEmbed[]**](CredentialsEmbed.md) | Embed credentials | [optional] 
**credentials_looker_openid** | [**\Swagger\Client\Looker\Model\CredentialsLookerOpenid**](CredentialsLookerOpenid.md) | LookerOpenID credentials. Used for login by Looker Analysts | [optional] 
**sessions** | [**\Swagger\Client\Looker\Model\Session[]**](Session.md) | Active sessions | [optional] 
**role_ids** | **int[]** | Array of ids of the roles for this user | [optional] 
**group_ids** | **int[]** | Array of ids of the groups for this user | [optional] 
**presumed_looker_employee** | **bool** | User is identified as an employee of Looker | [optional] 
**verified_looker_employee** | **bool** | User is identified as an employee of Looker who has been verified via Looker corporate authentication | [optional] 
**looker_versions** | **string[]** | Array of strings representing the Looker versions that this user has used (this only goes back as far as &#39;3.54.0&#39;) | [optional] 
**ui_state** | **map[string,string]** | Per user dictionary of undocumented state information owned by the Looker UI. | [optional] 
**locale** | **string** | User&#39;s preferred locale. User locale takes precedence over Looker&#39;s system-wide default locale. Locale determines language of display strings and date and numeric formatting in API responses. Locale string must be a 2 letter language code or a combination of language code and region code: &#39;en&#39; or &#39;en-US&#39;, for example. | [optional] 
**url** | **string** | Link to get this item | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



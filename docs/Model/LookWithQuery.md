# LookWithQuery

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**content_metadata_id** | **int** | Id of content metadata | [optional] 
**view_count** | **int** | Number of times viewed in the Looker web UI | [optional] 
**favorite_count** | **int** | Number of times favorited | [optional] 
**content_favorite_id** | **int** | Content Favorite Id | [optional] 
**title** | **string** | Look Title | [optional] 
**user** | [**\Swagger\Client\Model\UserIdOnly**](UserIdOnly.md) | User | [optional] 
**query_id** | **int** | Query Id | [optional] 
**description** | **string** | Description | [optional] 
**short_url** | **string** | Short Url | [optional] 
**space** | [**\Swagger\Client\Model\SpaceBase**](SpaceBase.md) | Space of this Look | [optional] 
**public** | **bool** | Is Public | [optional] 
**public_slug** | **string** | Public Slug | [optional] 
**user_id** | **int** | (Write-Only) User Id | [optional] 
**space_id** | **string** | (Write-Only) Space Id | [optional] 
**model** | [**\Swagger\Client\Model\LookModel**](LookModel.md) | Model | [optional] 
**public_url** | **string** | Public Url | [optional] 
**embed_url** | **string** | Embed Url | [optional] 
**google_spreadsheet_formula** | **string** | Google Spreadsheet Formula | [optional] 
**excel_file_url** | **string** | Excel File Url | [optional] 
**url** | **string** | Url | [optional] 
**query** | [**\Swagger\Client\Model\Query**](Query.md) | Query | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | Time that the Look was created. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | Time that the Look was updated. | [optional] 
**deleted_at** | [**\DateTime**](\DateTime.md) | Time that the Look was deleted. | [optional] 
**last_updater_id** | **int** | Id of User that last updated the look. | [optional] 
**last_viewed_at** | [**\DateTime**](\DateTime.md) | Time last viewed in the Looker web UI | [optional] 
**last_accessed_at** | [**\DateTime**](\DateTime.md) | Time that the Look was last accessed by any user | [optional] 
**deleter_id** | **int** | Id of User that deleted the look. | [optional] 
**deleted** | **bool** | Whether or not the look is deleted | [optional] 
**is_run_on_load** | **bool** | auto-run query when Look viewed | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# Look

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** | Unique Id | [optional] 
**content_metadata_id** | **int** | Id of content metadata | [optional] 
**view_count** | **int** | Number of times viewed in the Looker web UI | [optional] 
**favorite_count** | **int** | Number of times favorited | [optional] 
**last_accessed_at** | [**\DateTime**](\DateTime.md) | Time that the Look was last accessed by any user | [optional] 
**content_favorite_id** | **int** | Content Favorite Id | [optional] 
**title** | **string** | Look Title | [optional] 
**user** | [**\Looker\Model\UserIdOnly**](UserIdOnly.md) | User | [optional] 
**query_id** | **int** | Query Id | [optional] 
**description** | **string** | Description | [optional] 
**short_url** | **string** | Short Url | [optional] 
**space** | [**\Looker\Model\SpaceBase**](SpaceBase.md) | Space of this Look | [optional] 
**public** | **bool** | Is Public | [optional] 
**public_slug** | **string** | Public Slug | [optional] 
**user_id** | **int** | User Id | [optional] 
**space_id** | **string** | Space Id | [optional] 
**model** | [**\Looker\Model\LookModel**](LookModel.md) | Model | [optional] 
**public_url** | **string** | Public Url | [optional] 
**embed_url** | **string** | Embed Url | [optional] 
**image_embed_url** | **string** | Image Embed Url | [optional] 
**google_spreadsheet_formula** | **string** | Google Spreadsheet Formula | [optional] 
**excel_file_url** | **string** | Excel File Url | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | Time that the Look was created. | [optional] 
**deleted_at** | [**\DateTime**](\DateTime.md) | Time that the Look was deleted. | [optional] 
**updated_at** | [**\DateTime**](\DateTime.md) | Time that the Look was updated. | [optional] 
**last_updater_id** | **int** | Id of User that last updated the look. | [optional] 
**deleter_id** | **int** | Id of User that deleted the look. | [optional] 
**deleted** | **bool** | Whether or not a look is deleted. | [optional] 
**last_viewed_at** | [**\DateTime**](\DateTime.md) | Time last viewed in the Looker web UI | [optional] 
**is_run_on_load** | **bool** | auto-run query when Look viewed | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# HomepageItem

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**homepage_section_id** | **string** | Associated Homepage Section | [optional] 
**order** | **int** | An arbitrary integer representing the sort order within the section | [optional] 
**title** | **string** | The actual title for display | [optional] 
**custom_title** | **string** | Custom title entered by the user, if present | [optional] 
**use_custom_title** | **bool** | Whether the custom title should be used instead of the content title, if the item is associated with content | [optional] 
**description** | **string** | The actual description for display | [optional] 
**custom_description** | **string** | Custom description entered by the user, if present | [optional] 
**use_custom_description** | **bool** | Whether the custom description should be used instead of the content description, if the item is associated with content | [optional] 
**url** | **string** | The actual url for display | [optional] 
**custom_url** | **string** | Custom url entered by the user, if present | [optional] 
**use_custom_url** | **bool** | Whether the custom url should be used instead of the content url, if the item is associated with content | [optional] 
**image_url** | **string** | The actual image_url for display | [optional] 
**custom_image_url** | **string** | Custom image_url entered by the user, if present | [optional] 
**custom_image_data_base64** | **string** | (Write-Only) base64 encoded image data | [optional] 
**use_custom_image** | **bool** | Whether the custom image should be used instead of the content image, if the item is associated with content | [optional] 
**look_id** | **int** | Look to base this item on | [optional] 
**dashboard_id** | **int** | Dashboard to base this item on | [optional] 
**lookml_dashboard_id** | **string** | LookML Dashboard to base this item on | [optional] 
**view_count** | **int** | Number of times content has been viewed, if present | [optional] 
**favorite_count** | **int** | Number of times content has been favorited, if present | [optional] 
**content_created_by** | **string** | Name of user who created the content this item is based on | [optional] 
**content_updated_at** | **string** | Last time the content that this item is based on was updated | [optional] 
**content_favorite_id** | **int** | Content favorite id associated with the item this content is based on | [optional] 
**content_metadata_id** | **int** | Content metadata id associated with the item this content is based on | [optional] 
**section_fetch_time** | **float** | Number of seconds it took to fetch the section this item is in | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



# DashboardElement

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**dashboard_id** | **string** | Id of Dashboard | [optional] 
**look_id** | **string** | Id Of Look | [optional] 
**query_id** | **int** | Id Of Query | [optional] 
**type** | **string** | Type | [optional] 
**listen** | **map[string,string]** | Listen | [optional] 
**refresh_interval** | **string** | Refresh Interval | [optional] 
**refresh_interval_to_i** | **int** | Refresh Interval as integer | [optional] 
**note_text** | **string** | Note Text | [optional] 
**note_text_as_html** | **string** | Note Text as Html | [optional] 
**note_display** | **string** | Note Display | [optional] 
**note_state** | **string** | Note State | [optional] 
**title_hidden** | **bool** | Whether title is hidden | [optional] 
**title_text** | **string** | Text tile title | [optional] 
**title** | **string** | Title of dashboard element | [optional] 
**subtitle_text** | **string** | Text tile subtitle text | [optional] 
**body_text** | **string** | Text tile body text | [optional] 
**body_text_as_html** | **string** | Text tile body text as Html | [optional] 
**look** | [**\Swagger\Client\Looker\Model\LookWithQuery**](LookWithQuery.md) | Look | [optional] 
**query** | [**\Swagger\Client\Looker\Model\Query**](Query.md) | Query | [optional] 
**edit_uri** | **string** | Relative path of URI of LookML file to edit the dashboard element (LookML dashboard only). | [optional] 
**merge_result_id** | **string** | ID of merge result | [optional] 
**result_maker_id** | **int** | ID of the ResultMakerLookup entry. | [optional] 
**result_maker** | [**\Swagger\Client\Looker\Model\ResultMakerWithIdVisConfigAndDynamicFields**](ResultMakerWithIdVisConfigAndDynamicFields.md) | Data about the result maker. | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



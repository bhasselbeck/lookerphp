# DashboardBase

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**user_id** | **int** | Id of User | [optional] 
**title** | **string** | Look Title | [optional] 
**description** | **string** | Description | [optional] 
**readonly** | **bool** | Is Read-only | [optional] 
**hidden** | **bool** | Is Hidden | [optional] 
**refresh_interval** | **string** | Refresh Interval | [optional] 
**refresh_interval_to_i** | **int** | Refresh Interval as Integer | [optional] 
**space** | [**\Swagger\Client\Model\SpaceBase**](SpaceBase.md) | Space | [optional] 
**model** | [**\Swagger\Client\Model\LookModel**](LookModel.md) | Model | [optional] 
**content_favorite_id** | **int** | Content Favorite Id | [optional] 
**scheduled_plan** | [**\Swagger\Client\Model\ScheduledPlan**](ScheduledPlan.md) | ScheduledPlan | [optional] 
**content_metadata_id** | **int** | Id of content metadata | [optional] 
**query_timezone** | **string** | Timezone in which the Dashboard will run by default. | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



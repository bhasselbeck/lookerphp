# MergeQuery

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**pivots** | **string[]** | Pivots | [optional] 
**sorts** | **string[]** | Sorts | [optional] 
**column_limit** | **string** | Column Limit | [optional] 
**total** | **bool** | Total | [optional] 
**vis_config** | **map[string,string]** | Visualization Config | [optional] 
**dynamic_fields** | **string** | Dynamic Fields | [optional] 
**source_queries** | [**\Swagger\Client\Looker\Model\MergeQuerySourceQuery[]**](MergeQuerySourceQuery.md) | Source Queries defining the results to be merged. | [optional] 
**result_maker_id** | **int** | Unique to get results | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



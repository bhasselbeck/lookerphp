# DashboardFilter

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**dashboard_id** | **string** | Id of Dashboard | [optional] 
**name** | **string** | Name of filter | [optional] 
**title** | **string** | Title of filter | [optional] 
**type** | **string** | Type of filter: one of date, number, string, or field | [optional] 
**default_value** | **string** | Default value of filter | [optional] 
**model** | **string** | Model of filter (required if type &#x3D; field) | [optional] 
**explore** | **string** | Explore of filter (required if type &#x3D; field) | [optional] 
**dimension** | **string** | Dimension of filter (required if type &#x3D; field) | [optional] 
**field** | **map[string,string]** | Field information | [optional] 
**row** | **int** | Position of filter when displaying | [optional] 
**listens_to_filters** | **string[]** | Array of listeners for faceted filters | [optional] 
**allow_multiple_values** | **bool** | Whether the filter allows multiple filter values | [optional] 
**required** | **bool** | Whether the filter requires a value to run the dashboard | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



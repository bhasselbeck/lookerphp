# DialectInfo

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **string** | The name of the dialect | [optional] 
**label** | **string** | The human-readable label of the connection | [optional] 
**label_for_database_equivalent** | **string** | What the dialect calls the equivalent of a normal SQL table | [optional] 
**default_port** | **string** | Default port number | [optional] 
**default_max_connections** | **string** | Default number max connections | [optional] 
**supported_options** | [**\Swagger\Client\Model\DialectInfoOptions**](DialectInfoOptions.md) | Option support details | [optional] 
**installed** | **bool** | Is the supporting driver installed | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



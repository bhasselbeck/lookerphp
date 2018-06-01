# Dashboard

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **string** | Unique Id | [optional] 
**content_metadata_id** | **int** | Id of content metadata | [optional] 
**content_favorite_id** | **int** | Content Favorite Id | [optional] 
**view_count** | **int** | Number of times viewed in the Looker web UI | [optional] 
**last_accessed_at** | [**\DateTime**](\DateTime.md) | Time the dashboard was last accessed | [optional] 
**favorite_count** | **int** | Number of times favorited | [optional] 
**user_id** | **int** | Id of User | [optional] 
**title** | **string** | Look Title | [optional] 
**description** | **string** | Description | [optional] 
**readonly** | **bool** | Is Read-only | [optional] 
**hidden** | **bool** | Is Hidden | [optional] 
**refresh_interval** | **string** | Refresh Interval | [optional] 
**refresh_interval_to_i** | **int** | Refresh Interval as Integer | [optional] 
**space** | [**\Looker\Model\SpaceBase**](SpaceBase.md) | Space | [optional] 
**load_configuration** | **string** | configuration option that governs how dashboard loading will happen. | [optional] 
**model** | [**\Looker\Model\LookModel**](LookModel.md) | Model | [optional] 
**space_id** | **string** | Id of Space | [optional] 
**dashboard_elements** | [**\Looker\Model\DashboardElement[]**](DashboardElement.md) | Elements | [optional] 
**dashboard_layouts** | [**\Looker\Model\DashboardLayout[]**](DashboardLayout.md) | Layouts | [optional] 
**dashboard_filters** | [**\Looker\Model\DashboardFilter[]**](DashboardFilter.md) | Filters | [optional] 
**last_viewed_at** | [**\DateTime**](\DateTime.md) | Time last viewed in the Looker web UI | [optional] 
**background_color** | **string** | Background color | [optional] 
**show_title** | **bool** | Show title | [optional] 
**title_color** | **string** | Title color | [optional] 
**show_filters_bar** | **bool** | Show filters bar.  **Security Note:** This property only affects the *cosmetic* appearance of the dashboard, not a user&#39;Ls ability to access data. Hiding the filters bar does **NOT** prevent users from changing filters by other means. For information on how to set up secure data access control policies, see [Control User Access to Data](https://docs.looker.com/admin-options/tutorials/permissions#control_user_access_to_data) | [optional] 
**tile_background_color** | **string** | Tile background color | [optional] 
**tile_text_color** | **string** | Tile text color | [optional] 
**text_tile_text_color** | **string** | Color of text on text tiles | [optional] 
**last_updater_id** | **int** | Id of User that last updated the dashboard. | [optional] 
**deleter_id** | **int** | Id of User that deleted the dashboard. | [optional] 
**deleted** | **bool** | Whether or not a dashboard is deleted. | [optional] 
**created_at** | [**\DateTime**](\DateTime.md) | Time that the Dashboard was created. | [optional] 
**deleted_at** | [**\DateTime**](\DateTime.md) | Time that the Dashboard was deleted. | [optional] 
**query_timezone** | **string** | Timezone in which the Dashboard will run by default. | [optional] 
**edit_uri** | **string** | Relative path of URI of LookML file to edit the dashboard (LookML dashboard only). | [optional] 
**can** | **map[string,bool]** | Operations the current user is able to perform on this object | [optional] 

[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)



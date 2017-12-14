# Vimbox\RoomsApi\WorkbooksApi

All URIs are relative to *https://rooms.vimbox.dev-v4.skyeng.link*

Method | HTTP request | Description
------------- | ------------- | -------------
[**roomsServerApiV1WorkbooksNotStartedHwCountGet**](WorkbooksApi.md#roomsServerApiV1WorkbooksNotStartedHwCountGet) | **GET** /rooms/server-api/v1/workbooks/notStartedHwCount | Return count not started homeworks


# **roomsServerApiV1WorkbooksNotStartedHwCountGet**
> int roomsServerApiV1WorkbooksNotStartedHwCountGet($student_id)

Return count not started homeworks

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: BasicAuth
Vimbox\RoomsApi\Configuration::getDefaultConfiguration()->setUsername('YOUR_USERNAME');
Vimbox\RoomsApi\Configuration::getDefaultConfiguration()->setPassword('YOUR_PASSWORD');

$api_instance = new Vimbox\RoomsApi\Api\WorkbooksApi();
$student_id = "student_id_example"; // string | 

try {
    $result = $api_instance->roomsServerApiV1WorkbooksNotStartedHwCountGet($student_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling WorkbooksApi->roomsServerApiV1WorkbooksNotStartedHwCountGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **student_id** | **string**|  | [optional]

### Return type

**int**

### Authorization

[BasicAuth](../../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


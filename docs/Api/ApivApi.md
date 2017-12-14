# Vimbox\RoomsApi\ApivApi

All URIs are relative to *https://rooms.vimbox.dev-v4.skyeng.link*

Method | HTTP request | Description
------------- | ------------- | -------------
[**roomsServerApiV1WorkbooksByLessonsGet**](ApivApi.md#roomsServerApiV1WorkbooksByLessonsGet) | **GET** /rooms/server-api/v1/workbooks/byLessons | Return workbooks with provided lessonIds
[**roomsServerApiV1WorkbooksHwFindBelongerForStudentAndStepPairsPost**](ApivApi.md#roomsServerApiV1WorkbooksHwFindBelongerForStudentAndStepPairsPost) | **POST** /rooms/server-api/v1/workbooks/hw/findBelongerForStudentAndStepPairs | Найти \&quot;владельца\&quot;(ДЗ/Тест) для набора степ/студент.


# **roomsServerApiV1WorkbooksByLessonsGet**
> \Vimbox\RoomsApi\Model\WorkbookWithLastRoomDate[] roomsServerApiV1WorkbooksByLessonsGet($lesson_ids, $student_id)

Return workbooks with provided lessonIds

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: BasicAuth
Vimbox\RoomsApi\Configuration::getDefaultConfiguration()->setUsername('YOUR_USERNAME');
Vimbox\RoomsApi\Configuration::getDefaultConfiguration()->setPassword('YOUR_PASSWORD');

$api_instance = new Vimbox\RoomsApi\Api\ApivApi();
$lesson_ids = array("lesson_ids_example"); // string[] | Lesson ids
$student_id = 56; // int | Student id

try {
    $result = $api_instance->roomsServerApiV1WorkbooksByLessonsGet($lesson_ids, $student_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApivApi->roomsServerApiV1WorkbooksByLessonsGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **lesson_ids** | [**string[]**](../Model/string.md)| Lesson ids |
 **student_id** | **int**| Student id |

### Return type

[**\Vimbox\RoomsApi\Model\WorkbookWithLastRoomDate[]**](../Model/WorkbookWithLastRoomDate.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **roomsServerApiV1WorkbooksHwFindBelongerForStudentAndStepPairsPost**
> \Vimbox\RoomsApi\Model\Belonger[] roomsServerApiV1WorkbooksHwFindBelongerForStudentAndStepPairsPost($student_step_pairs)

Найти \"владельца\"(ДЗ/Тест) для набора степ/студент.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: BasicAuth
Vimbox\RoomsApi\Configuration::getDefaultConfiguration()->setUsername('YOUR_USERNAME');
Vimbox\RoomsApi\Configuration::getDefaultConfiguration()->setPassword('YOUR_PASSWORD');

$api_instance = new Vimbox\RoomsApi\Api\ApivApi();
$student_step_pairs = "student_step_pairs_example"; // string | 

try {
    $result = $api_instance->roomsServerApiV1WorkbooksHwFindBelongerForStudentAndStepPairsPost($student_step_pairs);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ApivApi->roomsServerApiV1WorkbooksHwFindBelongerForStudentAndStepPairsPost: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **student_step_pairs** | **string**|  |

### Return type

[**\Vimbox\RoomsApi\Model\Belonger[]**](../Model/Belonger.md)

### Authorization

[BasicAuth](../../README.md#BasicAuth)

### HTTP request headers

 - **Content-Type**: application/x-www-form-urlencoded
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


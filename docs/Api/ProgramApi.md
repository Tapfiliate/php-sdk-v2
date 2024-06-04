# Tapfiliate\Sdk\ProgramApi

All URIs are relative to **

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAListOfPrograms**](ProgramApi.md#getalistofprograms) | **GET** /api/program/ | 

# **getAListOfPrograms**
> \Tapfiliate\Sdk\Model\InlineResponse200 getAListOfPrograms($page, $limit)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
// Configure API key authorization: ApiKeyAuth
$config = Tapfiliate\Sdk\Configuration::getDefaultConfiguration()->setApiKey('X-Api-Key', 'YOUR_API_KEY');
// Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
// $config = Tapfiliate\Sdk\Configuration::getDefaultConfiguration()->setApiKeyPrefix('X-Api-Key', 'Bearer');

$apiInstance = new Tapfiliate\Sdk\Api\ProgramApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$page = 1; // int | 
$limit = 50; // int | 

try {
    $result = $apiInstance->getAListOfPrograms($page, $limit);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ProgramApi->getAListOfPrograms: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **int**|  | [optional] [default to 1]
 **limit** | **int**|  | [optional] [default to 50]

### Return type

[**\Tapfiliate\Sdk\Model\InlineResponse200**](../Model/InlineResponse200.md)

### Authorization

[ApiKeyAuth](../../README.md#ApiKeyAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


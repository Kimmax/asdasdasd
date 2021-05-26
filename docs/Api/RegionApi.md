# Swagger\Client\RegionApi

All URIs are relative to *https://localhost/api/beta*

Method | HTTP request | Description
------------- | ------------- | -------------
[**regionsCountryIdGet**](RegionApi.md#regionsCountryIdGet) | **GET** /regions/{country_id} | Get list of regions with name and country_id


# **regionsCountryIdGet**
> \Swagger\Client\Model\InlineResponse2008 regionsCountryIdGet($country_id)

Get list of regions with name and country_id

Get all regions

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

// Configure HTTP basic authorization: basicAuth
$config = Swagger\Client\Configuration::getDefaultConfiguration()
              ->setUsername('YOUR_USERNAME')
              ->setPassword('YOUR_PASSWORD');


$apiInstance = new Swagger\Client\Api\RegionApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$country_id = 56; // int | ID of country to return country regions

try {
    $result = $apiInstance->regionsCountryIdGet($country_id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling RegionApi->regionsCountryIdGet: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **country_id** | **int**| ID of country to return country regions |

### Return type

[**\Swagger\Client\Model\InlineResponse2008**](../Model/InlineResponse2008.md)

### Authorization

[basicAuth](../../README.md#basicAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


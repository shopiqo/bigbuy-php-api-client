# Efsa\Client\Bigbuy\ShippingAPIApi

All URIs are relative to https://api.bigbuy.eu.

Method | HTTP request | Description
------------- | ------------- | -------------
[**getTheListOfAvailableCarriers()**](ShippingAPIApi.md#getTheListOfAvailableCarriers) | **GET** /rest/shipping/carriers.{_format} | Get the list of available carriers


## `getTheListOfAvailableCarriers()`

```php
getTheListOfAvailableCarriers($format)
```

Get the list of available carriers

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\ShippingAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getTheListOfAvailableCarriers($format);
} catch (Exception $e) {
    echo 'Exception when calling ShippingAPIApi->getTheListOfAvailableCarriers: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]

### Return type

void (empty response body)

### Authorization

[API_KEY](../../README.md#API_KEY)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

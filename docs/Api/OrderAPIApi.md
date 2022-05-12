# Efsa\Client\Bigbuy\OrderAPIApi

All URIs are relative to https://api.bigbuy.eu.

Method | HTTP request | Description
------------- | ------------- | -------------
[**getOrderCarriersStructure()**](OrderAPIApi.md#getOrderCarriersStructure) | **GET** /rest/order/carriers/new.{_format} | Get order carriers structure
[**getOrderShippingAddressStructure()**](OrderAPIApi.md#getOrderShippingAddressStructure) | **GET** /rest/order/addresses/new.{_format} | Get order shipping address structure


## `getOrderCarriersStructure()`

```php
getOrderCarriersStructure($format)
```

Get order carriers structure

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\OrderAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getOrderCarriersStructure($format);
} catch (Exception $e) {
    echo 'Exception when calling OrderAPIApi->getOrderCarriersStructure: ', $e->getMessage(), PHP_EOL;
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

## `getOrderShippingAddressStructure()`

```php
getOrderShippingAddressStructure($format)
```

Get order shipping address structure

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\OrderAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getOrderShippingAddressStructure($format);
} catch (Exception $e) {
    echo 'Exception when calling OrderAPIApi->getOrderShippingAddressStructure: ', $e->getMessage(), PHP_EOL;
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

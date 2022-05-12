# Efsa\Client\Bigbuy\TrackingAPIApi

All URIs are relative to https://api.bigbuy.eu.

Method | HTTP request | Description
------------- | ------------- | -------------
[**getTheListOfAvailableTrackings()**](TrackingAPIApi.md#getTheListOfAvailableTrackings) | **GET** /rest/tracking/carriers.{_format} | Get the list of available trackings
[**getTheListOfAvailableTrackingsForThePassedOrdersYaml()**](TrackingAPIApi.md#getTheListOfAvailableTrackingsForThePassedOrdersYaml) | **POST** /rest/tracking/orders.{_format} | Get the list of available trackings for the passed orders.
[**getTrackingStatusByOrderId()**](TrackingAPIApi.md#getTrackingStatusByOrderId) | **GET** /rest/tracking/order/{id}.{_format} | Get tracking status by order id


## `getTheListOfAvailableTrackings()`

```php
getTheListOfAvailableTrackings($format)
```

Get the list of available trackings

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\TrackingAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getTheListOfAvailableTrackings($format);
} catch (Exception $e) {
    echo 'Exception when calling TrackingAPIApi->getTheListOfAvailableTrackings: ', $e->getMessage(), PHP_EOL;
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

## `getTheListOfAvailableTrackingsForThePassedOrdersYaml()`

```php
getTheListOfAvailableTrackingsForThePassedOrdersYaml($format)
```

Get the list of available trackings for the passed orders.

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\TrackingAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getTheListOfAvailableTrackingsForThePassedOrdersYaml($format);
} catch (Exception $e) {
    echo 'Exception when calling TrackingAPIApi->getTheListOfAvailableTrackingsForThePassedOrdersYaml: ', $e->getMessage(), PHP_EOL;
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

## `getTrackingStatusByOrderId()`

```php
getTrackingStatusByOrderId($id, $format)
```

Get tracking status by order id

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\TrackingAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string

try {
    $apiInstance->getTrackingStatusByOrderId($id, $format);
} catch (Exception $e) {
    echo 'Exception when calling TrackingAPIApi->getTrackingStatusByOrderId: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
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

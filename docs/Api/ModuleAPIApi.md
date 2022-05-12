# Efsa\Client\Bigbuy\ModuleAPIApi

All URIs are relative to https://api.bigbuy.eu.

Method | HTTP request | Description
------------- | ------------- | -------------
[**getAllModules()**](ModuleAPIApi.md#getAllModules) | **GET** /rest/module/.{_format} | Get all Modules
[**getAllModulesPlatforms()**](ModuleAPIApi.md#getAllModulesPlatforms) | **GET** /rest/module/platforms.{_format} | Get all module platforms


## `getAllModules()`

```php
getAllModules($format, $name, $platform, $platformVersion)
```

Get all Modules

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\ModuleAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$name = 'name_example'; // string | Module name
$platform = 'platform_example'; // string | Platform name
$platformVersion = 'platformVersion_example'; // string | Platform version

try {
    $apiInstance->getAllModules($format, $name, $platform, $platformVersion);
} catch (Exception $e) {
    echo 'Exception when calling ModuleAPIApi->getAllModules: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **name** | **string**| Module name | [optional]
 **platform** | **string**| Platform name | [optional]
 **platformVersion** | **string**| Platform version | [optional]

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

## `getAllModulesPlatforms()`

```php
getAllModulesPlatforms($format, $name, $platform, $platformVersion)
```

Get all module platforms

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\ModuleAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$name = 'name_example'; // string | Module name
$platform = 'platform_example'; // string | Platform name
$platformVersion = 'platformVersion_example'; // string | Platform version

try {
    $apiInstance->getAllModulesPlatforms($format, $name, $platform, $platformVersion);
} catch (Exception $e) {
    echo 'Exception when calling ModuleAPIApi->getAllModulesPlatforms: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **name** | **string**| Module name | [optional]
 **platform** | **string**| Platform name | [optional]
 **platformVersion** | **string**| Platform version | [optional]

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

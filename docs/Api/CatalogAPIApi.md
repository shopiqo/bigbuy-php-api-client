# Efsa\Client\Bigbuy\CatalogAPIApi

All URIs are relative to https://api.bigbuy.eu.

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCatalogAttribute()**](CatalogAPIApi.md#getCatalogAttribute) | **GET** /rest/catalog/attribute/{id}.{_format} | Get a single attribute
[**getCatalogAttributeGroup()**](CatalogAPIApi.md#getCatalogAttributeGroup) | **GET** /rest/catalog/attributegroup/{id}.{_format} | Get a single attribute group
[**getCatalogAttributeGroups()**](CatalogAPIApi.md#getCatalogAttributeGroups) | **GET** /rest/catalog/attributegroups.{_format} | Lists all attribute groups
[**getCatalogAttributeLanguages()**](CatalogAPIApi.md#getCatalogAttributeLanguages) | **GET** /rest/catalog/attributealllanguages/{id}.{_format} | Get languages of a single attribute
[**getCatalogAttributegroupalllanguages()**](CatalogAPIApi.md#getCatalogAttributegroupalllanguages) | **GET** /rest/catalog/attributegroupalllanguages/{id}.{_format} | Get all languages of a single attribute group
[**getCatalogCategories()**](CatalogAPIApi.md#getCatalogCategories) | **GET** /rest/catalog/categories.{_format} | Lists all categories
[**getCatalogCategory()**](CatalogAPIApi.md#getCatalogCategory) | **GET** /rest/catalog/category/{id}.{_format} | Returns the selected category
[**getCatalogCategoryalllanguages()**](CatalogAPIApi.md#getCatalogCategoryalllanguages) | **GET** /rest/catalog/categoryalllanguages/{id}.{_format} | Lists all categories
[**getCatalogLanguages()**](CatalogAPIApi.md#getCatalogLanguages) | **GET** /rest/catalog/languages.{_format} | Returns all languages
[**getCatalogManufacturer()**](CatalogAPIApi.md#getCatalogManufacturer) | **GET** /rest/catalog/manufacturer/{id}.{_format} | Get a single manufacturer
[**getCatalogManufacturers()**](CatalogAPIApi.md#getCatalogManufacturers) | **GET** /rest/catalog/manufacturers.{_format} | Returns all manufacturers
[**getCatalogProduct()**](CatalogAPIApi.md#getCatalogProduct) | **GET** /rest/catalog/product/{id}.{_format} | Returns the selected product
[**getCatalogProductcategories()**](CatalogAPIApi.md#getCatalogProductcategories) | **GET** /rest/catalog/productcategories/{id}.{_format} | Get product categories
[**getCatalogProductimages()**](CatalogAPIApi.md#getCatalogProductimages) | **GET** /rest/catalog/productimages/{id}.{_format} | Get a single product images
[**getCatalogProductinformation()**](CatalogAPIApi.md#getCatalogProductinformation) | **GET** /rest/catalog/productinformation/{id}.{_format} | Get a single product
[**getCatalogProductinformationalllanguages()**](CatalogAPIApi.md#getCatalogProductinformationalllanguages) | **GET** /rest/catalog/productinformationalllanguages/{id}.{_format} | Get a single product
[**getCatalogProductinformationbysku()**](CatalogAPIApi.md#getCatalogProductinformationbysku) | **GET** /rest/catalog/productinformationbysku/{sku}.{_format} | Get a single product by sku
[**getCatalogProducts()**](CatalogAPIApi.md#getCatalogProducts) | **GET** /rest/catalog/products.{_format} | Returns all products
[**getCatalogProductsinformation()**](CatalogAPIApi.md#getCatalogProductsinformation) | **GET** /rest/catalog/productsinformation.{_format} | Returns all products
[**getCatalogProductsstock()**](CatalogAPIApi.md#getCatalogProductsstock) | **GET** /rest/catalog/productsstock.{_format} | Returns all products stock
[**getCatalogProductsstockavailable()**](CatalogAPIApi.md#getCatalogProductsstockavailable) | **GET** /rest/catalog/productsstockavailable.{_format} | Returns all products with available stock
[**getCatalogProductsstockbyreference()**](CatalogAPIApi.md#getCatalogProductsstockbyreference) | **POST** /rest/catalog/productsstockbyreference.{_format} | Returns all selected products stock
[**getCatelogAttributes()**](CatalogAPIApi.md#getCatelogAttributes) | **GET** /rest/catalog/attributes.{_format} | Lists all attributes


## `getCatalogAttribute()`

```php
getCatalogAttribute($id, $format, $isoCode)
```

Get a single attribute

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogAttribute($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogAttribute: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogAttributeGroup()`

```php
getCatalogAttributeGroup($id, $format, $isoCode)
```

Get a single attribute group

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogAttributeGroup($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogAttributeGroup: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogAttributeGroups()`

```php
getCatalogAttributeGroups($format, $isoCode)
```

Lists all attribute groups

Rate limit: 24 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogAttributeGroups($format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogAttributeGroups: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogAttributeLanguages()`

```php
getCatalogAttributeLanguages($id, $format, $isoCode)
```

Get languages of a single attribute

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogAttributeLanguages($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogAttributeLanguages: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogAttributegroupalllanguages()`

```php
getCatalogAttributegroupalllanguages($id, $format)
```

Get all languages of a single attribute group

Rate limit: 1 request(s) in 1 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string

try {
    $apiInstance->getCatalogAttributegroupalllanguages($id, $format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogAttributegroupalllanguages: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogCategories()`

```php
getCatalogCategories($format, $isoCode)
```

Lists all categories

Rate limit: 24 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogCategories($format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogCategories: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogCategory()`

```php
getCatalogCategory($id, $format, $isoCode)
```

Returns the selected category

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogCategory($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogCategory: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogCategoryalllanguages()`

```php
getCatalogCategoryalllanguages($id, $format, $isoCode)
```

Lists all categories

Rate limit: 24 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogCategoryalllanguages($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogCategoryalllanguages: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogLanguages()`

```php
getCatalogLanguages($format)
```

Returns all languages

Rate limit: 10 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getCatalogLanguages($format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogLanguages: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogManufacturer()`

```php
getCatalogManufacturer($id, $format)
```

Get a single manufacturer

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string

try {
    $apiInstance->getCatalogManufacturer($id, $format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogManufacturer: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogManufacturers()`

```php
getCatalogManufacturers($format)
```

Returns all manufacturers

Rate limit: 5 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getCatalogManufacturers($format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogManufacturers: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogProduct()`

```php
getCatalogProduct($id, $format, $isoCode)
```

Returns the selected product

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogProduct($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProduct: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogProductcategories()`

```php
getCatalogProductcategories($id, $format)
```

Get product categories

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string

try {
    $apiInstance->getCatalogProductcategories($id, $format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductcategories: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogProductimages()`

```php
getCatalogProductimages($id, $format)
```

Get a single product images

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string

try {
    $apiInstance->getCatalogProductimages($id, $format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductimages: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogProductinformation()`

```php
getCatalogProductinformation($id, $format, $isoCode)
```

Get a single product

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogProductinformation($id, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductinformation: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogProductinformationalllanguages()`

```php
getCatalogProductinformationalllanguages($id, $format)
```

Get a single product

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$id = 56; // int
$format = json; // string

try {
    $apiInstance->getCatalogProductinformationalllanguages($id, $format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductinformationalllanguages: ', $e->getMessage(), PHP_EOL;
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

## `getCatalogProductinformationbysku()`

```php
getCatalogProductinformationbysku($sku, $format, $isoCode)
```

Get a single product by sku

Rate limit: 1 request(s) in 5 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$sku = 'sku_example'; // string
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatalogProductinformationbysku($sku, $format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductinformationbysku: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sku** | **string**|  |
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogProducts()`

```php
getCatalogProducts($format, $pageSize, $page, $isoCode)
```

Returns all products

Rate limit: 10 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$pageSize = 56; // int | Page size
$page = 56; // int | Page
$isoCode = de; // string

try {
    $apiInstance->getCatalogProducts($format, $pageSize, $page, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProducts: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **pageSize** | **int**| Page size |
 **page** | **int**| Page |
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogProductsinformation()`

```php
getCatalogProductsinformation($format, $page, $pageSize, $isoCode)
```

Returns all products

Rate limit: 24 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$page = 56; // int | Page
$pageSize = 56; // int | Page size
$isoCode = de; // string

try {
    $apiInstance->getCatalogProductsinformation($format, $page, $pageSize, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductsinformation: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **page** | **int**| Page |
 **pageSize** | **int**| Page size |
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

## `getCatalogProductsstock()`

```php
getCatalogProductsstock($format, $page, $pageSize)
```

Returns all products stock

Rate limit: 10 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$page = 56; // int | Page
$pageSize = 56; // int | Page size

try {
    $apiInstance->getCatalogProductsstock($format, $page, $pageSize);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductsstock: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **page** | **int**| Page |
 **pageSize** | **int**| Page size |

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

## `getCatalogProductsstockavailable()`

```php
getCatalogProductsstockavailable($format, $page, $pageSize)
```

Returns all products with available stock

Rate limit: 10 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$page = 56; // int | Page
$pageSize = 56; // int | Page size

try {
    $apiInstance->getCatalogProductsstockavailable($format, $page, $pageSize);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductsstockavailable: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **page** | **int**| Page |
 **pageSize** | **int**| Page size |

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

## `getCatalogProductsstockbyreference()`

```php
getCatalogProductsstockbyreference($format)
```

Returns all selected products stock

Rate limit: 25 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string

try {
    $apiInstance->getCatalogProductsstockbyreference($format);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatalogProductsstockbyreference: ', $e->getMessage(), PHP_EOL;
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

## `getCatelogAttributes()`

```php
getCatelogAttributes($format, $isoCode)
```

Lists all attributes

Rate limit: 24 request(s) in 3600 second(s)

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: API_KEY
$config = Efsa\Client\Bigbuy\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Efsa\Client\Bigbuy\Api\CatalogAPIApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$format = json; // string
$isoCode = de; // string

try {
    $apiInstance->getCatelogAttributes($format, $isoCode);
} catch (Exception $e) {
    echo 'Exception when calling CatalogAPIApi->getCatelogAttributes: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **format** | **string**|  | [default to &#39;json&#39;]
 **isoCode** | **string**|  | [optional] [default to &#39;de&#39;]

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

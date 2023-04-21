# REST client for BigBuy

OpenAPI spefication to interact with bigbuy.eu


## Installation & Usage

### Requirements

PHP 7.3 and later.
Should also work with PHP 8.0 or 8.1 but has not been tested.

### Composer

To install the bindings via [Composer](https://getcomposer.org/), add the following to `composer.json`:

```json
{
  "repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/shopiqo/bigbuy-php-api-client.git"
    }
  ],
  "require": {
    "shopiqo/bigbuy-php-api-client": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
<?php
require_once('/path/to/REST client for BigBuy/vendor/autoload.php');
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

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

## API Endpoints

All URIs are relative to *https://api.bigbuy.eu*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*CatalogAPIApi* | [**getCatalogAttribute**](docs/Api/CatalogAPIApi.md#getcatalogattribute) | **GET** /rest/catalog/attribute/{id}.{_format} | Get a single attribute
*CatalogAPIApi* | [**getCatalogAttributeGroup**](docs/Api/CatalogAPIApi.md#getcatalogattributegroup) | **GET** /rest/catalog/attributegroup/{id}.{_format} | Get a single attribute group
*CatalogAPIApi* | [**getCatalogAttributeGroups**](docs/Api/CatalogAPIApi.md#getcatalogattributegroups) | **GET** /rest/catalog/attributegroups.{_format} | Lists all attribute groups
*CatalogAPIApi* | [**getCatalogAttributeLanguages**](docs/Api/CatalogAPIApi.md#getcatalogattributelanguages) | **GET** /rest/catalog/attributealllanguages/{id}.{_format} | Get languages of a single attribute
*CatalogAPIApi* | [**getCatalogAttributegroupalllanguages**](docs/Api/CatalogAPIApi.md#getcatalogattributegroupalllanguages) | **GET** /rest/catalog/attributegroupalllanguages/{id}.{_format} | Get all languages of a single attribute group
*CatalogAPIApi* | [**getCatalogCategories**](docs/Api/CatalogAPIApi.md#getcatalogcategories) | **GET** /rest/catalog/categories.{_format} | Lists all categories
*CatalogAPIApi* | [**getCatalogCategory**](docs/Api/CatalogAPIApi.md#getcatalogcategory) | **GET** /rest/catalog/category/{id}.{_format} | Returns the selected category
*CatalogAPIApi* | [**getCatalogCategoryalllanguages**](docs/Api/CatalogAPIApi.md#getcatalogcategoryalllanguages) | **GET** /rest/catalog/categoryalllanguages/{id}.{_format} | Lists all categories
*CatalogAPIApi* | [**getCatalogLanguages**](docs/Api/CatalogAPIApi.md#getcataloglanguages) | **GET** /rest/catalog/languages.{_format} | Returns all languages
*CatalogAPIApi* | [**getCatalogManufacturer**](docs/Api/CatalogAPIApi.md#getcatalogmanufacturer) | **GET** /rest/catalog/manufacturer/{id}.{_format} | Get a single manufacturer
*CatalogAPIApi* | [**getCatalogManufacturers**](docs/Api/CatalogAPIApi.md#getcatalogmanufacturers) | **GET** /rest/catalog/manufacturers.{_format} | Returns all manufacturers
*CatalogAPIApi* | [**getCatalogProduct**](docs/Api/CatalogAPIApi.md#getcatalogproduct) | **GET** /rest/catalog/product/{id}.{_format} | Returns the selected product
*CatalogAPIApi* | [**getCatalogProductcategories**](docs/Api/CatalogAPIApi.md#getcatalogproductcategories) | **GET** /rest/catalog/productcategories/{id}.{_format} | Get product categories
*CatalogAPIApi* | [**getCatalogProductimages**](docs/Api/CatalogAPIApi.md#getcatalogproductimages) | **GET** /rest/catalog/productimages/{id}.{_format} | Get a single product images
*CatalogAPIApi* | [**getCatalogProductinformation**](docs/Api/CatalogAPIApi.md#getcatalogproductinformation) | **GET** /rest/catalog/productinformation/{id}.{_format} | Get a single product
*CatalogAPIApi* | [**getCatalogProductinformationalllanguages**](docs/Api/CatalogAPIApi.md#getcatalogproductinformationalllanguages) | **GET** /rest/catalog/productinformationalllanguages/{id}.{_format} | Get a single product
*CatalogAPIApi* | [**getCatalogProductinformationbysku**](docs/Api/CatalogAPIApi.md#getcatalogproductinformationbysku) | **GET** /rest/catalog/productinformationbysku/{sku}.{_format} | Get a single product by sku
*CatalogAPIApi* | [**getCatalogProducts**](docs/Api/CatalogAPIApi.md#getcatalogproducts) | **GET** /rest/catalog/products.{_format} | Returns all products
*CatalogAPIApi* | [**getCatalogProductsinformation**](docs/Api/CatalogAPIApi.md#getcatalogproductsinformation) | **GET** /rest/catalog/productsinformation.{_format} | Returns all products
*CatalogAPIApi* | [**getCatalogProductsstock**](docs/Api/CatalogAPIApi.md#getcatalogproductsstock) | **GET** /rest/catalog/productsstock.{_format} | Returns all products stock
*CatalogAPIApi* | [**getCatalogProductsstockavailable**](docs/Api/CatalogAPIApi.md#getcatalogproductsstockavailable) | **GET** /rest/catalog/productsstockavailable.{_format} | Returns all products with available stock
*CatalogAPIApi* | [**getCatalogProductsstockbyreference**](docs/Api/CatalogAPIApi.md#getcatalogproductsstockbyreference) | **POST** /rest/catalog/productsstockbyreference.{_format} | Returns all selected products stock
*CatalogAPIApi* | [**getCatelogAttributes**](docs/Api/CatalogAPIApi.md#getcatelogattributes) | **GET** /rest/catalog/attributes.{_format} | Lists all attributes
*ModuleAPIApi* | [**getAllModules**](docs/Api/ModuleAPIApi.md#getallmodules) | **GET** /rest/module/.{_format} | Get all Modules
*ModuleAPIApi* | [**getAllModulesPlatforms**](docs/Api/ModuleAPIApi.md#getallmodulesplatforms) | **GET** /rest/module/platforms.{_format} | Get all module platforms
*OrderAPIApi* | [**getOrderCarriersStructure**](docs/Api/OrderAPIApi.md#getordercarriersstructure) | **GET** /rest/order/carriers/new.{_format} | Get order carriers structure
*OrderAPIApi* | [**getOrderShippingAddressStructure**](docs/Api/OrderAPIApi.md#getordershippingaddressstructure) | **GET** /rest/order/addresses/new.{_format} | Get order shipping address structure
*ShippingAPIApi* | [**getTheListOfAvailableCarriers**](docs/Api/ShippingAPIApi.md#getthelistofavailablecarriers) | **GET** /rest/shipping/carriers.{_format} | Get the list of available carriers
*TrackingAPIApi* | [**getTheListOfAvailableTrackings**](docs/Api/TrackingAPIApi.md#getthelistofavailabletrackings) | **GET** /rest/tracking/carriers.{_format} | Get the list of available trackings
*TrackingAPIApi* | [**getTheListOfAvailableTrackingsForThePassedOrdersYaml**](docs/Api/TrackingAPIApi.md#getthelistofavailabletrackingsforthepassedordersyaml) | **POST** /rest/tracking/orders.{_format} | Get the list of available trackings for the passed orders.
*TrackingAPIApi* | [**getTrackingStatusByOrderId**](docs/Api/TrackingAPIApi.md#gettrackingstatusbyorderid) | **GET** /rest/tracking/order/{id}.{_format} | Get tracking status by order id

## Models


## Authorization

### API_KEY

- **Type**: Bearer authentication

## Tests

To run the tests, use:

```bash
composer install
vendor/bin/phpunit
```

## Author



## About this package

This PHP package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: `v202102`
    - Package version: `1.0.0`
- Build package: `org.openapitools.codegen.languages.PhpClientCodegen`

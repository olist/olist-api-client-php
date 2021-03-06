# SwaggerClient-php
No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)

This PHP package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:

- API version: v1
- Build package: io.swagger.codegen.languages.PhpClientCodegen

## Requirements

PHP 5.4.0 and later

## Installation & Usage
### Composer

To install the bindings via [Composer](http://getcomposer.org/), add the following to `composer.json`:

```
{
  "repositories": [
    {
      "type": "git",
      "url": "https://github.com/GIT_USER_ID/GIT_REPO_ID.git"
    }
  ],
  "require": {
    "GIT_USER_ID/GIT_REPO_ID": "*@dev"
  }
}
```

Then run `composer install`

### Manual Installation

Download the files and include `autoload.php`:

```php
    require_once('/path/to/SwaggerClient-php/autoload.php');
```

## Tests

To run the unit tests:

```
composer install
./vendor/bin/phpunit
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$limit = "limit_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 
$offset = "offset_example"; // string | 

try {
    $api_instance->itemsBySkuList($authorization, $limit, $ordering, $search, $offset);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->itemsBySkuList: ', $e->getMessage(), PHP_EOL;
}

?>
```

## Documentation for API Endpoints

All URIs are relative to *https://api.olist.com/v1*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*DefaultApi* | [**itemsBySkuList**](docs/Api/DefaultApi.md#itemsbyskulist) | **GET** /items-by-sku | 
*DefaultApi* | [**productGroupsCreate**](docs/Api/DefaultApi.md#productgroupscreate) | **POST** /product-groups | 
*DefaultApi* | [**productGroupsDelete**](docs/Api/DefaultApi.md#productgroupsdelete) | **DELETE** /product-groups/{id} | 
*DefaultApi* | [**productGroupsList**](docs/Api/DefaultApi.md#productgroupslist) | **GET** /product-groups | 
*DefaultApi* | [**productGroupsPartialUpdate**](docs/Api/DefaultApi.md#productgroupspartialupdate) | **PATCH** /product-groups/{id} | 
*DefaultApi* | [**productGroupsRead**](docs/Api/DefaultApi.md#productgroupsread) | **GET** /product-groups/{id} | 
*DefaultApi* | [**productGroupsUpdate**](docs/Api/DefaultApi.md#productgroupsupdate) | **PUT** /product-groups/{id} | 
*DefaultApi* | [**productsCreate**](docs/Api/DefaultApi.md#productscreate) | **POST** /template/products | 
*DefaultApi* | [**productsDelete**](docs/Api/DefaultApi.md#productsdelete) | **DELETE** /template/products/{gtin} | 
*DefaultApi* | [**productsList**](docs/Api/DefaultApi.md#productslist) | **GET** /template/products | 
*DefaultApi* | [**productsPartialUpdate**](docs/Api/DefaultApi.md#productspartialupdate) | **PATCH** /template/products/{gtin} | 
*DefaultApi* | [**productsRead**](docs/Api/DefaultApi.md#productsread) | **GET** /template/products/{gtin} | 
*DefaultApi* | [**productsUpdate**](docs/Api/DefaultApi.md#productsupdate) | **PUT** /template/products/{gtin} | 
*DefaultApi* | [**sellerOrdersCreate**](docs/Api/DefaultApi.md#sellerorderscreate) | **POST** /seller-orders | 
*DefaultApi* | [**sellerOrdersDelete**](docs/Api/DefaultApi.md#sellerordersdelete) | **DELETE** /seller-orders/{code} | 
*DefaultApi* | [**sellerOrdersItemsList**](docs/Api/DefaultApi.md#sellerordersitemslist) | **GET** /seller-orders-items | 
*DefaultApi* | [**sellerOrdersItemsRead**](docs/Api/DefaultApi.md#sellerordersitemsread) | **GET** /seller-orders-items/{id} | 
*DefaultApi* | [**sellerOrdersList**](docs/Api/DefaultApi.md#sellerorderslist) | **GET** /seller-orders | 
*DefaultApi* | [**sellerOrdersPartialUpdate**](docs/Api/DefaultApi.md#sellerorderspartialupdate) | **PATCH** /seller-orders/{code} | 
*DefaultApi* | [**sellerOrdersRead**](docs/Api/DefaultApi.md#sellerordersread) | **GET** /seller-orders/{code} | 
*DefaultApi* | [**sellerOrdersShipment**](docs/Api/DefaultApi.md#sellerordersshipment) | **PUT** /seller-orders/{code}/shipment | 
*DefaultApi* | [**sellerOrdersUpdate**](docs/Api/DefaultApi.md#sellerordersupdate) | **PUT** /seller-orders/{code} | 
*DefaultApi* | [**sellerProductsCreate**](docs/Api/DefaultApi.md#sellerproductscreate) | **POST** /seller-products | 
*DefaultApi* | [**sellerProductsDelete**](docs/Api/DefaultApi.md#sellerproductsdelete) | **DELETE** /seller-products/{sku} | 
*DefaultApi* | [**sellerProductsHistoryList**](docs/Api/DefaultApi.md#sellerproductshistorylist) | **GET** /seller-products-history | 
*DefaultApi* | [**sellerProductsHistoryRead**](docs/Api/DefaultApi.md#sellerproductshistoryread) | **GET** /seller-products-history/{seller_product__sku} | 
*DefaultApi* | [**sellerProductsList**](docs/Api/DefaultApi.md#sellerproductslist) | **GET** /seller-products | 
*DefaultApi* | [**sellerProductsPartialUpdate**](docs/Api/DefaultApi.md#sellerproductspartialupdate) | **PATCH** /seller-products/{sku} | 
*DefaultApi* | [**sellerProductsRead**](docs/Api/DefaultApi.md#sellerproductsread) | **GET** /seller-products/{sku} | 
*DefaultApi* | [**sellerProductsUpdate**](docs/Api/DefaultApi.md#sellerproductsupdate) | **PUT** /seller-products/{sku} | 
*DefaultApi* | [**sellersCreate**](docs/Api/DefaultApi.md#sellerscreate) | **POST** /sellers | 
*DefaultApi* | [**sellersDelete**](docs/Api/DefaultApi.md#sellersdelete) | **DELETE** /sellers/{id} | 
*DefaultApi* | [**sellersList**](docs/Api/DefaultApi.md#sellerslist) | **GET** /sellers | 
*DefaultApi* | [**sellersPartialUpdate**](docs/Api/DefaultApi.md#sellerspartialupdate) | **PATCH** /sellers/{id} | 
*DefaultApi* | [**sellersRead**](docs/Api/DefaultApi.md#sellersread) | **GET** /sellers/{id} | 
*DefaultApi* | [**sellersUpdate**](docs/Api/DefaultApi.md#sellersupdate) | **PUT** /sellers/{id} | 
*DefaultApi* | [**statsRead**](docs/Api/DefaultApi.md#statsread) | **GET** /_stats/orders/{seller_id} | 
*DefaultApi* | [**statsRead_0**](docs/Api/DefaultApi.md#statsread_0) | **GET** /_stats/products/{seller_id} | 
*DefaultApi* | [**usersCreate**](docs/Api/DefaultApi.md#userscreate) | **POST** /users | 
*DefaultApi* | [**usersDelete**](docs/Api/DefaultApi.md#usersdelete) | **DELETE** /users/{id} | 
*DefaultApi* | [**usersList**](docs/Api/DefaultApi.md#userslist) | **GET** /users | 
*DefaultApi* | [**usersPartialUpdate**](docs/Api/DefaultApi.md#userspartialupdate) | **PATCH** /users/{id} | 
*DefaultApi* | [**usersRead**](docs/Api/DefaultApi.md#usersread) | **GET** /users/{id} | 
*DefaultApi* | [**usersUpdate**](docs/Api/DefaultApi.md#usersupdate) | **PUT** /users/{id} | 


## Documentation For Models

 - [MODEL053815](docs/Model/MODEL053815.md)
 - [MODEL0cb980](docs/Model/MODEL0cb980.md)
 - [MODEL2eaa59](docs/Model/MODEL2eaa59.md)
 - [MODEL3efebe](docs/Model/MODEL3efebe.md)
 - [MODEL40d2ff](docs/Model/MODEL40d2ff.md)
 - [MODEL4339e0](docs/Model/MODEL4339e0.md)
 - [MODEL686451](docs/Model/MODEL686451.md)
 - [MODEL6c172d](docs/Model/MODEL6c172d.md)
 - [MODEL70b893](docs/Model/MODEL70b893.md)
 - [MODEL871628](docs/Model/MODEL871628.md)
 - [MODEL8779bd](docs/Model/MODEL8779bd.md)
 - [MODELae14ae](docs/Model/MODELae14ae.md)
 - [MODELbc7b75](docs/Model/MODELbc7b75.md)
 - [MODELc30ccf](docs/Model/MODELc30ccf.md)
 - [MODELd4278c](docs/Model/MODELd4278c.md)
 - [MODELeaf0a6](docs/Model/MODELeaf0a6.md)
 - [MODELf3a1b6](docs/Model/MODELf3a1b6.md)
 - [MODELf585b9](docs/Model/MODELf585b9.md)
 - [MODELfa9d13](docs/Model/MODELfa9d13.md)


## Documentation For Authorization

 All endpoints do not require authorization.


## Author





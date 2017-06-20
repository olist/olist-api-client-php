# Swagger\Client\DefaultApi

All URIs are relative to *https://api.olist.com/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**itemsBySkuList**](DefaultApi.md#itemsBySkuList) | **GET** /items-by-sku | 
[**productGroupsCreate**](DefaultApi.md#productGroupsCreate) | **POST** /product-groups | 
[**productGroupsDelete**](DefaultApi.md#productGroupsDelete) | **DELETE** /product-groups/{id} | 
[**productGroupsList**](DefaultApi.md#productGroupsList) | **GET** /product-groups | 
[**productGroupsPartialUpdate**](DefaultApi.md#productGroupsPartialUpdate) | **PATCH** /product-groups/{id} | 
[**productGroupsRead**](DefaultApi.md#productGroupsRead) | **GET** /product-groups/{id} | 
[**productGroupsUpdate**](DefaultApi.md#productGroupsUpdate) | **PUT** /product-groups/{id} | 
[**productsCreate**](DefaultApi.md#productsCreate) | **POST** /template/products | 
[**productsDelete**](DefaultApi.md#productsDelete) | **DELETE** /template/products/{gtin} | 
[**productsList**](DefaultApi.md#productsList) | **GET** /template/products | 
[**productsPartialUpdate**](DefaultApi.md#productsPartialUpdate) | **PATCH** /template/products/{gtin} | 
[**productsRead**](DefaultApi.md#productsRead) | **GET** /template/products/{gtin} | 
[**productsUpdate**](DefaultApi.md#productsUpdate) | **PUT** /template/products/{gtin} | 
[**sellerOrdersCreate**](DefaultApi.md#sellerOrdersCreate) | **POST** /seller-orders | 
[**sellerOrdersDelete**](DefaultApi.md#sellerOrdersDelete) | **DELETE** /seller-orders/{code} | 
[**sellerOrdersItemsList**](DefaultApi.md#sellerOrdersItemsList) | **GET** /seller-orders-items | 
[**sellerOrdersItemsRead**](DefaultApi.md#sellerOrdersItemsRead) | **GET** /seller-orders-items/{id} | 
[**sellerOrdersList**](DefaultApi.md#sellerOrdersList) | **GET** /seller-orders | 
[**sellerOrdersPartialUpdate**](DefaultApi.md#sellerOrdersPartialUpdate) | **PATCH** /seller-orders/{code} | 
[**sellerOrdersRead**](DefaultApi.md#sellerOrdersRead) | **GET** /seller-orders/{code} | 
[**sellerOrdersShipment**](DefaultApi.md#sellerOrdersShipment) | **PUT** /seller-orders/{code}/shipment | 
[**sellerOrdersUpdate**](DefaultApi.md#sellerOrdersUpdate) | **PUT** /seller-orders/{code} | 
[**sellerProductsCreate**](DefaultApi.md#sellerProductsCreate) | **POST** /seller-products | 
[**sellerProductsDelete**](DefaultApi.md#sellerProductsDelete) | **DELETE** /seller-products/{sku} | 
[**sellerProductsHistoryList**](DefaultApi.md#sellerProductsHistoryList) | **GET** /seller-products-history | 
[**sellerProductsHistoryRead**](DefaultApi.md#sellerProductsHistoryRead) | **GET** /seller-products-history/{seller_product__sku} | 
[**sellerProductsList**](DefaultApi.md#sellerProductsList) | **GET** /seller-products | 
[**sellerProductsPartialUpdate**](DefaultApi.md#sellerProductsPartialUpdate) | **PATCH** /seller-products/{sku} | 
[**sellerProductsRead**](DefaultApi.md#sellerProductsRead) | **GET** /seller-products/{sku} | 
[**sellerProductsUpdate**](DefaultApi.md#sellerProductsUpdate) | **PUT** /seller-products/{sku} | 
[**sellersCreate**](DefaultApi.md#sellersCreate) | **POST** /sellers | 
[**sellersDelete**](DefaultApi.md#sellersDelete) | **DELETE** /sellers/{id} | 
[**sellersList**](DefaultApi.md#sellersList) | **GET** /sellers | 
[**sellersPartialUpdate**](DefaultApi.md#sellersPartialUpdate) | **PATCH** /sellers/{id} | 
[**sellersRead**](DefaultApi.md#sellersRead) | **GET** /sellers/{id} | 
[**sellersUpdate**](DefaultApi.md#sellersUpdate) | **PUT** /sellers/{id} | 
[**statsRead**](DefaultApi.md#statsRead) | **GET** /_stats/orders/{seller_id} | 
[**statsRead_0**](DefaultApi.md#statsRead_0) | **GET** /_stats/products/{seller_id} | 
[**usersCreate**](DefaultApi.md#usersCreate) | **POST** /users | 
[**usersDelete**](DefaultApi.md#usersDelete) | **DELETE** /users/{id} | 
[**usersList**](DefaultApi.md#usersList) | **GET** /users | 
[**usersPartialUpdate**](DefaultApi.md#usersPartialUpdate) | **PATCH** /users/{id} | 
[**usersRead**](DefaultApi.md#usersRead) | **GET** /users/{id} | 
[**usersUpdate**](DefaultApi.md#usersUpdate) | **PUT** /users/{id} | 


# **itemsBySkuList**
> itemsBySkuList($authorization, $limit, $ordering, $search, $offset)



### Example
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

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **limit** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]
 **offset** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productGroupsCreate**
> productGroupsCreate($authorization, $mode_leaf0a6)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$mode_leaf0a6 = new \Swagger\Client\Model\MODELeaf0a6(); // \Swagger\Client\Model\MODELeaf0a6 | 

try {
    $api_instance->productGroupsCreate($authorization, $mode_leaf0a6);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productGroupsCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **mode_leaf0a6** | [**\Swagger\Client\Model\MODELeaf0a6**](../Model/\Swagger\Client\Model\MODELeaf0a6.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productGroupsDelete**
> productGroupsDelete($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->productGroupsDelete($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productGroupsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productGroupsList**
> productGroupsList($authorization, $limit, $ordering, $search, $offset)



### Example
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
    $api_instance->productGroupsList($authorization, $limit, $ordering, $search, $offset);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productGroupsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **limit** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]
 **offset** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productGroupsPartialUpdate**
> productGroupsPartialUpdate($authorization, $id, $mode_lf585b9)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 
$mode_lf585b9 = new \Swagger\Client\Model\MODELf585b9(); // \Swagger\Client\Model\MODELf585b9 | 

try {
    $api_instance->productGroupsPartialUpdate($authorization, $id, $mode_lf585b9);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productGroupsPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |
 **mode_lf585b9** | [**\Swagger\Client\Model\MODELf585b9**](../Model/\Swagger\Client\Model\MODELf585b9.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productGroupsRead**
> productGroupsRead($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->productGroupsRead($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productGroupsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productGroupsUpdate**
> productGroupsUpdate($authorization, $id, $model0cb980)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 
$model0cb980 = new \Swagger\Client\Model\MODEL0cb980(); // \Swagger\Client\Model\MODEL0cb980 | 

try {
    $api_instance->productGroupsUpdate($authorization, $id, $model0cb980);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productGroupsUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |
 **model0cb980** | [**\Swagger\Client\Model\MODEL0cb980**](../Model/\Swagger\Client\Model\MODEL0cb980.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productsCreate**
> productsCreate($authorization, $mode_lc30ccf)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$mode_lc30ccf = new \Swagger\Client\Model\MODELc30ccf(); // \Swagger\Client\Model\MODELc30ccf | 

try {
    $api_instance->productsCreate($authorization, $mode_lc30ccf);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productsCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **mode_lc30ccf** | [**\Swagger\Client\Model\MODELc30ccf**](../Model/\Swagger\Client\Model\MODELc30ccf.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productsDelete**
> productsDelete($gtin, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$gtin = "gtin_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->productsDelete($gtin, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gtin** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productsList**
> productsList($authorization, $limit, $gtin, $name__icontains, $name, $offset, $ordering, $search)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$limit = "limit_example"; // string | 
$gtin = "gtin_example"; // string | 
$name__icontains = "name__icontains_example"; // string | 
$name = "name_example"; // string | 
$offset = "offset_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 

try {
    $api_instance->productsList($authorization, $limit, $gtin, $name__icontains, $name, $offset, $ordering, $search);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **limit** | **string**|  | [optional]
 **gtin** | **string**|  | [optional]
 **name__icontains** | **string**|  | [optional]
 **name** | **string**|  | [optional]
 **offset** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productsPartialUpdate**
> productsPartialUpdate($gtin, $authorization, $mode_lfa9d13)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$gtin = "gtin_example"; // string | 
$authorization = "authorization_example"; // string | 
$mode_lfa9d13 = new \Swagger\Client\Model\MODELfa9d13(); // \Swagger\Client\Model\MODELfa9d13 | 

try {
    $api_instance->productsPartialUpdate($gtin, $authorization, $mode_lfa9d13);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productsPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gtin** | **string**|  |
 **authorization** | **string**|  |
 **mode_lfa9d13** | [**\Swagger\Client\Model\MODELfa9d13**](../Model/\Swagger\Client\Model\MODELfa9d13.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productsRead**
> productsRead($gtin, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$gtin = "gtin_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->productsRead($gtin, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gtin** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **productsUpdate**
> productsUpdate($gtin, $authorization, $mode_lbc7b75)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$gtin = "gtin_example"; // string | 
$authorization = "authorization_example"; // string | 
$mode_lbc7b75 = new \Swagger\Client\Model\MODELbc7b75(); // \Swagger\Client\Model\MODELbc7b75 | 

try {
    $api_instance->productsUpdate($gtin, $authorization, $mode_lbc7b75);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->productsUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gtin** | **string**|  |
 **authorization** | **string**|  |
 **mode_lbc7b75** | [**\Swagger\Client\Model\MODELbc7b75**](../Model/\Swagger\Client\Model\MODELbc7b75.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersCreate**
> sellerOrdersCreate($authorization, $mode_ld4278c)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$mode_ld4278c = new \Swagger\Client\Model\MODELd4278c(); // \Swagger\Client\Model\MODELd4278c | 

try {
    $api_instance->sellerOrdersCreate($authorization, $mode_ld4278c);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **mode_ld4278c** | [**\Swagger\Client\Model\MODELd4278c**](../Model/\Swagger\Client\Model\MODELd4278c.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersDelete**
> sellerOrdersDelete($code, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$code = "code_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->sellerOrdersDelete($code, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersItemsList**
> sellerOrdersItemsList($authorization, $seller_order, $limit, $ordering, $search, $offset)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$seller_order = "seller_order_example"; // string | 
$limit = "limit_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 
$offset = "offset_example"; // string | 

try {
    $api_instance->sellerOrdersItemsList($authorization, $seller_order, $limit, $ordering, $search, $offset);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersItemsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **seller_order** | **string**|  | [optional]
 **limit** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]
 **offset** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersItemsRead**
> sellerOrdersItemsRead($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->sellerOrdersItemsRead($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersItemsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersList**
> sellerOrdersList($authorization, $seller_id, $start_date, $overdue, $status, $code, $ordering, $search, $canceled, $limit, $order_id, $offset, $cancelation_status)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$seller_id = "seller_id_example"; // string | 
$start_date = "start_date_example"; // string | 
$overdue = "overdue_example"; // string | 
$status = "status_example"; // string | 
$code = "code_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 
$canceled = "canceled_example"; // string | 
$limit = "limit_example"; // string | 
$order_id = "order_id_example"; // string | 
$offset = "offset_example"; // string | 
$cancelation_status = "cancelation_status_example"; // string | 

try {
    $api_instance->sellerOrdersList($authorization, $seller_id, $start_date, $overdue, $status, $code, $ordering, $search, $canceled, $limit, $order_id, $offset, $cancelation_status);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **seller_id** | **string**|  | [optional]
 **start_date** | **string**|  | [optional]
 **overdue** | **string**|  | [optional]
 **status** | **string**|  | [optional]
 **code** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]
 **canceled** | **string**|  | [optional]
 **limit** | **string**|  | [optional]
 **order_id** | **string**|  | [optional]
 **offset** | **string**|  | [optional]
 **cancelation_status** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersPartialUpdate**
> sellerOrdersPartialUpdate($code, $authorization, $mode_lf3a1b6)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$code = "code_example"; // string | 
$authorization = "authorization_example"; // string | 
$mode_lf3a1b6 = new \Swagger\Client\Model\MODELf3a1b6(); // \Swagger\Client\Model\MODELf3a1b6 | 

try {
    $api_instance->sellerOrdersPartialUpdate($code, $authorization, $mode_lf3a1b6);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **string**|  |
 **authorization** | **string**|  |
 **mode_lf3a1b6** | [**\Swagger\Client\Model\MODELf3a1b6**](../Model/\Swagger\Client\Model\MODELf3a1b6.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersRead**
> sellerOrdersRead($code, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$code = "code_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->sellerOrdersRead($code, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersShipment**
> sellerOrdersShipment($code, $authorization, $model6c172d)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$code = "code_example"; // string | 
$authorization = "authorization_example"; // string | 
$model6c172d = new \Swagger\Client\Model\MODEL6c172d(); // \Swagger\Client\Model\MODEL6c172d | 

try {
    $api_instance->sellerOrdersShipment($code, $authorization, $model6c172d);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersShipment: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **string**|  |
 **authorization** | **string**|  |
 **model6c172d** | [**\Swagger\Client\Model\MODEL6c172d**](../Model/\Swagger\Client\Model\MODEL6c172d.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerOrdersUpdate**
> sellerOrdersUpdate($code, $authorization, $model8779bd)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$code = "code_example"; // string | 
$authorization = "authorization_example"; // string | 
$model8779bd = new \Swagger\Client\Model\MODEL8779bd(); // \Swagger\Client\Model\MODEL8779bd | 

try {
    $api_instance->sellerOrdersUpdate($code, $authorization, $model8779bd);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerOrdersUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **string**|  |
 **authorization** | **string**|  |
 **model8779bd** | [**\Swagger\Client\Model\MODEL8779bd**](../Model/\Swagger\Client\Model\MODEL8779bd.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsCreate**
> sellerProductsCreate($authorization, $model2eaa59)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$model2eaa59 = new \Swagger\Client\Model\MODEL2eaa59(); // \Swagger\Client\Model\MODEL2eaa59 | 

try {
    $api_instance->sellerProductsCreate($authorization, $model2eaa59);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **model2eaa59** | [**\Swagger\Client\Model\MODEL2eaa59**](../Model/\Swagger\Client\Model\MODEL2eaa59.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsDelete**
> sellerProductsDelete($authorization, $sku)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$sku = "sku_example"; // string | 

try {
    $api_instance->sellerProductsDelete($authorization, $sku);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **sku** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsHistoryList**
> sellerProductsHistoryList($authorization, $limit, $offset, $status, $ordering, $search, $seller_product__group)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$limit = "limit_example"; // string | 
$offset = "offset_example"; // string | 
$status = "status_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 
$seller_product__group = "seller_product__group_example"; // string | 

try {
    $api_instance->sellerProductsHistoryList($authorization, $limit, $offset, $status, $ordering, $search, $seller_product__group);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsHistoryList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **limit** | **string**|  | [optional]
 **offset** | **string**|  | [optional]
 **status** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]
 **seller_product__group** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsHistoryRead**
> sellerProductsHistoryRead($seller_product__sku, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$seller_product__sku = "seller_product__sku_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->sellerProductsHistoryRead($seller_product__sku, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsHistoryRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **seller_product__sku** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsList**
> sellerProductsList($authorization, $seller_id, $name, $canonical_sku, $status, $ordering, $search, $stock__quantity, $limit, $gtin, $name__icontains, $offset, $group, $has_canonical, $canonicals_by_name)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$seller_id = "seller_id_example"; // string | 
$name = "name_example"; // string | 
$canonical_sku = "canonical_sku_example"; // string | 
$status = "status_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 
$stock__quantity = "stock__quantity_example"; // string | 
$limit = "limit_example"; // string | 
$gtin = "gtin_example"; // string | 
$name__icontains = "name__icontains_example"; // string | 
$offset = "offset_example"; // string | 
$group = "group_example"; // string | 
$has_canonical = "has_canonical_example"; // string | 
$canonicals_by_name = "canonicals_by_name_example"; // string | 

try {
    $api_instance->sellerProductsList($authorization, $seller_id, $name, $canonical_sku, $status, $ordering, $search, $stock__quantity, $limit, $gtin, $name__icontains, $offset, $group, $has_canonical, $canonicals_by_name);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **seller_id** | **string**|  | [optional]
 **name** | **string**|  | [optional]
 **canonical_sku** | **string**|  | [optional]
 **status** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]
 **stock__quantity** | **string**|  | [optional]
 **limit** | **string**|  | [optional]
 **gtin** | **string**|  | [optional]
 **name__icontains** | **string**|  | [optional]
 **offset** | **string**|  | [optional]
 **group** | **string**|  | [optional]
 **has_canonical** | **string**|  | [optional]
 **canonicals_by_name** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsPartialUpdate**
> sellerProductsPartialUpdate($authorization, $sku, $model4339e0)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$sku = "sku_example"; // string | 
$model4339e0 = new \Swagger\Client\Model\MODEL4339e0(); // \Swagger\Client\Model\MODEL4339e0 | 

try {
    $api_instance->sellerProductsPartialUpdate($authorization, $sku, $model4339e0);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **sku** | **string**|  |
 **model4339e0** | [**\Swagger\Client\Model\MODEL4339e0**](../Model/\Swagger\Client\Model\MODEL4339e0.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsRead**
> sellerProductsRead($authorization, $sku)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$sku = "sku_example"; // string | 

try {
    $api_instance->sellerProductsRead($authorization, $sku);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **sku** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellerProductsUpdate**
> sellerProductsUpdate($authorization, $sku, $model871628)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$sku = "sku_example"; // string | 
$model871628 = new \Swagger\Client\Model\MODEL871628(); // \Swagger\Client\Model\MODEL871628 | 

try {
    $api_instance->sellerProductsUpdate($authorization, $sku, $model871628);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellerProductsUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **sku** | **string**|  |
 **model871628** | [**\Swagger\Client\Model\MODEL871628**](../Model/\Swagger\Client\Model\MODEL871628.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellersCreate**
> sellersCreate($authorization, $model3efebe)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$model3efebe = new \Swagger\Client\Model\MODEL3efebe(); // \Swagger\Client\Model\MODEL3efebe | 

try {
    $api_instance->sellersCreate($authorization, $model3efebe);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellersCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **model3efebe** | [**\Swagger\Client\Model\MODEL3efebe**](../Model/\Swagger\Client\Model\MODEL3efebe.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellersDelete**
> sellersDelete($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->sellersDelete($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellersDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellersList**
> sellersList($authorization, $owner__email, $limit, $offset, $blocked, $paused, $ordering, $search)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$owner__email = "owner__email_example"; // string | 
$limit = "limit_example"; // string | 
$offset = "offset_example"; // string | 
$blocked = "blocked_example"; // string | 
$paused = "paused_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 

try {
    $api_instance->sellersList($authorization, $owner__email, $limit, $offset, $blocked, $paused, $ordering, $search);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellersList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **owner__email** | **string**|  | [optional]
 **limit** | **string**|  | [optional]
 **offset** | **string**|  | [optional]
 **blocked** | **string**|  | [optional]
 **paused** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellersPartialUpdate**
> sellersPartialUpdate($authorization, $id, $model053815)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 
$model053815 = new \Swagger\Client\Model\MODEL053815(); // \Swagger\Client\Model\MODEL053815 | 

try {
    $api_instance->sellersPartialUpdate($authorization, $id, $model053815);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellersPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |
 **model053815** | [**\Swagger\Client\Model\MODEL053815**](../Model/\Swagger\Client\Model\MODEL053815.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellersRead**
> sellersRead($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->sellersRead($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellersRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **sellersUpdate**
> sellersUpdate($authorization, $id, $model686451)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 
$model686451 = new \Swagger\Client\Model\MODEL686451(); // \Swagger\Client\Model\MODEL686451 | 

try {
    $api_instance->sellersUpdate($authorization, $id, $model686451);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->sellersUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |
 **model686451** | [**\Swagger\Client\Model\MODEL686451**](../Model/\Swagger\Client\Model\MODEL686451.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **statsRead**
> statsRead($seller_id, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$seller_id = "seller_id_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->statsRead($seller_id, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->statsRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **seller_id** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **statsRead_0**
> statsRead_0($seller_id, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$seller_id = "seller_id_example"; // string | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->statsRead_0($seller_id, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->statsRead_0: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **seller_id** | **string**|  |
 **authorization** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **usersCreate**
> usersCreate($authorization, $model40d2ff)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$model40d2ff = new \Swagger\Client\Model\MODEL40d2ff(); // \Swagger\Client\Model\MODEL40d2ff | 

try {
    $api_instance->usersCreate($authorization, $model40d2ff);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->usersCreate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **model40d2ff** | [**\Swagger\Client\Model\MODEL40d2ff**](../Model/\Swagger\Client\Model\MODEL40d2ff.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **usersDelete**
> usersDelete($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->usersDelete($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->usersDelete: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **usersList**
> usersList($authorization, $email, $limit, $name, $offset, $ordering, $search)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$email = "email_example"; // string | 
$limit = "limit_example"; // string | 
$name = "name_example"; // string | 
$offset = "offset_example"; // string | 
$ordering = "ordering_example"; // string | 
$search = "search_example"; // string | 

try {
    $api_instance->usersList($authorization, $email, $limit, $name, $offset, $ordering, $search);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->usersList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **email** | **string**|  | [optional]
 **limit** | **string**|  | [optional]
 **name** | **string**|  | [optional]
 **offset** | **string**|  | [optional]
 **ordering** | **string**|  | [optional]
 **search** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **usersPartialUpdate**
> usersPartialUpdate($id, $mode_lae14ae, $authorization)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$id = "id_example"; // string | 
$mode_lae14ae = new \Swagger\Client\Model\MODELae14ae(); // \Swagger\Client\Model\MODELae14ae | 
$authorization = "authorization_example"; // string | 

try {
    $api_instance->usersPartialUpdate($id, $mode_lae14ae, $authorization);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->usersPartialUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **string**|  |
 **mode_lae14ae** | [**\Swagger\Client\Model\MODELae14ae**](../Model/\Swagger\Client\Model\MODELae14ae.md)|  |
 **authorization** | **string**|  | [optional]

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **usersRead**
> usersRead($authorization, $id)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 

try {
    $api_instance->usersRead($authorization, $id);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->usersRead: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **usersUpdate**
> usersUpdate($authorization, $id, $model70b893)



### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\DefaultApi();
$authorization = "authorization_example"; // string | 
$id = "id_example"; // string | 
$model70b893 = new \Swagger\Client\Model\MODEL70b893(); // \Swagger\Client\Model\MODEL70b893 | 

try {
    $api_instance->usersUpdate($authorization, $id, $model70b893);
} catch (Exception $e) {
    echo 'Exception when calling DefaultApi->usersUpdate: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **authorization** | **string**|  |
 **id** | **string**|  |
 **model70b893** | [**\Swagger\Client\Model\MODEL70b893**](../Model/\Swagger\Client\Model\MODEL70b893.md)|  |

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


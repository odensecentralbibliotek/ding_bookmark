# Swagger\Client\ListApi

All URIs are relative to *https://prod.materiallist.dandigbib.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addListMaterial**](ListApi.md#addlistmaterial) | **PUT** /list/{listId}/{materialId} | 
[**checkListMaterial**](ListApi.md#checklistmaterial) | **HEAD** /list/{listId}/{materialId} | 
[**deleteListMaterial**](ListApi.md#deletelistmaterial) | **DELETE** /list/{listId}/{materialId} | 
[**getList**](ListApi.md#getlist) | **GET** /list/{listId} | 

# **addListMaterial**
> addListMaterial($list_id, $material_id)



Add material to the the list.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: BearerAuth
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\materiallistapi\ListApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$list_id = new \Swagger\Client\meteriallistclient\ListId(); // \Swagger\Client\meteriallistclient\ListId | The identifier of the list to return. Use \"default\" for the default list.
$material_id = new \Swagger\Client\meteriallistclient\MaterialId(); // \Swagger\Client\meteriallistclient\MaterialId | The identifier of the material.

try {
    $apiInstance->addListMaterial($list_id, $material_id);
} catch (Exception $e) {
    echo 'Exception when calling ListApi->addListMaterial: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | [**\Swagger\Client\meteriallistclient\ListId**](../Model/.md)| The identifier of the list to return. Use \&quot;default\&quot; for the default list. |
 **material_id** | [**\Swagger\Client\meteriallistclient\MaterialId**](../Model/.md)| The identifier of the material. |

### Return type

void (empty response body)

### Authorization

[BearerAuth](../../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **checkListMaterial**
> checkListMaterial($list_id, $material_id)



Check existence of material on list. To check multiple materials in one request, see the material_ids query parameter on /list/{listId}.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: BearerAuth
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\materiallistapi\ListApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$list_id = new \Swagger\Client\meteriallistclient\ListId(); // \Swagger\Client\meteriallistclient\ListId | The identifier of the list to return. Use \"default\" for the default list.
$material_id = new \Swagger\Client\meteriallistclient\MaterialId(); // \Swagger\Client\meteriallistclient\MaterialId | The identifier of the material.

try {
    $apiInstance->checkListMaterial($list_id, $material_id);
} catch (Exception $e) {
    echo 'Exception when calling ListApi->checkListMaterial: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | [**\Swagger\Client\meteriallistclient\ListId**](../Model/.md)| The identifier of the list to return. Use \&quot;default\&quot; for the default list. |
 **material_id** | [**\Swagger\Client\meteriallistclient\MaterialId**](../Model/.md)| The identifier of the material. |

### Return type

void (empty response body)

### Authorization

[BearerAuth](../../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **deleteListMaterial**
> deleteListMaterial($list_id, $material_id)



Delete material from list.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: BearerAuth
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\materiallistapi\ListApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$list_id = new \Swagger\Client\meteriallistclient\ListId(); // \Swagger\Client\meteriallistclient\ListId | The identifier of the list to return. Use \"default\" for the default list.
$material_id = new \Swagger\Client\meteriallistclient\MaterialId(); // \Swagger\Client\meteriallistclient\MaterialId | The identifier of the material.

try {
    $apiInstance->deleteListMaterial($list_id, $material_id);
} catch (Exception $e) {
    echo 'Exception when calling ListApi->deleteListMaterial: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | [**\Swagger\Client\meteriallistclient\ListId**](../Model/.md)| The identifier of the list to return. Use \&quot;default\&quot; for the default list. |
 **material_id** | [**\Swagger\Client\meteriallistclient\MaterialId**](../Model/.md)| The identifier of the material. |

### Return type

void (empty response body)

### Authorization

[BearerAuth](../../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **getList**
> \Swagger\Client\meteriallistclient\ModelList getList($list_id, $material_ids)



Get list with materials.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: BearerAuth
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\materiallistapi\ListApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$list_id = new \Swagger\Client\meteriallistclient\ListId(); // \Swagger\Client\meteriallistclient\ListId | The identifier of the list to return. Use \"default\" for the default list.
$material_ids = array(new \Swagger\Client\meteriallistclient\MaterialId()); // \Swagger\Client\meteriallistclient\MaterialId[] | Filter the list reply down to the given material identifiers. This is the recommended way to check for existence of multiple materials on the list.

try {
    $result = $apiInstance->getList($list_id, $material_ids);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling ListApi->getList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **list_id** | [**\Swagger\Client\meteriallistclient\ListId**](../Model/.md)| The identifier of the list to return. Use \&quot;default\&quot; for the default list. |
 **material_ids** | [**\Swagger\Client\meteriallistclient\MaterialId[]**](../Model/\Swagger\Client\meteriallistclient\MaterialId.md)| Filter the list reply down to the given material identifiers. This is the recommended way to check for existence of multiple materials on the list. | [optional]

### Return type

[**\Swagger\Client\meteriallistclient\ModelList**](../Model/ModelList.md)

### Authorization

[BearerAuth](../../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


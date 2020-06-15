# Swagger\Client\MigrateApi

All URIs are relative to *https://prod.materiallist.dandigbib.org*

Method | HTTP request | Description
------------- | ------------- | -------------
[**migrateList**](MigrateApi.md#migratelist) | **PUT** /migrate/{legacyUserId} | 

# **migrateList**
> migrateList($legacy_user_id)



Migrate list for the legacy user identifier to current user.

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');
    // Configure HTTP bearer authorization: BearerAuth
    $config = Swagger\Client\Configuration::getDefaultConfiguration()
    ->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new Swagger\Client\materiallistapi\MigrateApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$legacy_user_id = new \Swagger\Client\meteriallistclient\LegacyUserId(); // \Swagger\Client\meteriallistclient\LegacyUserId | Legacy user identifier of a migrated list.

try {
    $apiInstance->migrateList($legacy_user_id);
} catch (Exception $e) {
    echo 'Exception when calling MigrateApi->migrateList: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **legacy_user_id** | [**\Swagger\Client\meteriallistclient\LegacyUserId**](../Model/.md)| Legacy user identifier of a migrated list. |

### Return type

void (empty response body)

### Authorization

[BearerAuth](../../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)


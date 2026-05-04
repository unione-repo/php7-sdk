# UniOne\SystemApi

All URIs are relative to https://api.unione.io/en/transactional/api/v1

Method | HTTP request | Description
------------- | ------------- | -------------
[**systemInfo()**](SystemApi.md#systemInfo) | **POST** /system/info.json | Gets user or project info by API key.
[**systemPing()**](SystemApi.md#systemPing) | **POST** /system/ping.json | Checks API key validity and returns user ID.


## `systemInfo()`

```php
systemInfo(): \UniOne\Model\SystemInfo200Response
```

Gets user or project info by API key.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: apiKeyAuth
$config = UniOne\Configuration::getDefaultConfiguration()->setApiKey('X-API-KEY', 'YOUR_API_KEY');
$config->setHost('api.unione.io')


$apiInstance = new UniOne\Api\SystemApi(
    // If you want use custom http client, pass your client which implements `Psr\Http\Client\ClientInterface`.
    // This is optional, `Psr18ClientDiscovery` will be used to find http client. For instance `GuzzleHttp\Client` implements that interface
    new GuzzleHttp\Client(),
    $config
);


try {
    $result = $apiInstance->systemInfo();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SystemApi->systemInfo: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\UniOne\Model\SystemInfo200Response**](../Model/SystemInfo200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `systemPing()`

```php
systemPing(): \UniOne\Model\SystemPing200Response
```

Checks API key validity and returns user ID.

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure API key authorization: apiKeyAuth
$config = UniOne\Configuration::getDefaultConfiguration()->setApiKey('X-API-KEY', 'YOUR_API_KEY');
$config->setHost('api.unione.io')


$apiInstance = new UniOne\Api\SystemApi(
    // If you want use custom http client, pass your client which implements `Psr\Http\Client\ClientInterface`.
    // This is optional, `Psr18ClientDiscovery` will be used to find http client. For instance `GuzzleHttp\Client` implements that interface
    new GuzzleHttp\Client(),
    $config
);


try {
    $result = $apiInstance->systemPing();
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling SystemApi->systemPing: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**\UniOne\Model\SystemPing200Response**](../Model/SystemPing200Response.md)

### Authorization

[apiKeyAuth](../../README.md#apiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

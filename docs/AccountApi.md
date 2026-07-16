# WhoisFreaks.AccountApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**accountUsage**](AccountApi.md#accountUsage) | **GET** /v1.0/whoisapi/usage | Account Usage
[**databaseFileStatus**](AccountApi.md#databaseFileStatus) | **GET** /v3.3/status | Database File Status (Public)
[**rotateApiKey**](AccountApi.md#rotateApiKey) | **GET** /v1.0/api-key/rotate | Rotate API Key



## accountUsage

> AccountUsageResponse accountUsage()

Account Usage

Account Usage. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.AccountApi();
apiInstance.accountUsage().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

[**AccountUsageResponse**](AccountUsageResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## databaseFileStatus

> DatabaseFileStatus databaseFileStatus()

Database File Status (Public)

No API key required. Returns freshness of all downloadable files.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';

let apiInstance = new WhoisFreaks.AccountApi();
apiInstance.databaseFileStatus().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

[**DatabaseFileStatus**](DatabaseFileStatus.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## rotateApiKey

> String rotateApiKey()

Rotate API Key

Rotate API Key. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.AccountApi();
apiInstance.rotateApiKey().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

**String**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain


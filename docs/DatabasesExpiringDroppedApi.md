# WhoisFreaks.DatabasesExpiringDroppedApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbDropped**](DatabasesExpiringDroppedApi.md#dbDropped) | **GET** /v3.1/download/domainer/dropped | Dropped Domains
[**dbDroppedBacklinks**](DatabasesExpiringDroppedApi.md#dbDroppedBacklinks) | **GET** /v3.3/download/domainer/dropped/backlinks | Dropped With Backlinks
[**dbDroppedJson**](DatabasesExpiringDroppedApi.md#dbDroppedJson) | **GET** /v3.1/domains/dropped | Dropped Domains (JSON)
[**dbExpired**](DatabasesExpiringDroppedApi.md#dbExpired) | **GET** /v3.1/download/domainer/expired | Expiring Domains
[**dbExpiredCleaned**](DatabasesExpiringDroppedApi.md#dbExpiredCleaned) | **GET** /v3.1/download/domainer/expired/cleaned | Expiring Cleaned WHOIS



## dbDropped

> Blob dbDropped(whois, opts)

Dropped Domains

Dropped Domains. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesExpiringDroppedApi();
let whois = true; // Boolean | 
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbDropped(whois, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **whois** | **Boolean**|  | 
 **date** | **Date**| yyyy-MM-dd; omit for latest | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbDroppedBacklinks

> Blob dbDroppedBacklinks(opts)

Dropped With Backlinks

Dropped With Backlinks. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesExpiringDroppedApi();
let opts = {
  'whois': true, // Boolean | 
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbDroppedBacklinks(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **whois** | **Boolean**|  | [optional] 
 **date** | **Date**| yyyy-MM-dd; omit for latest | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbDroppedJson

> [String] dbDroppedJson(opts)

Dropped Domains (JSON)

Dropped Domains (JSON). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesExpiringDroppedApi();
let opts = {
  'date': new Date("2026-10-01"), // Date | yyyy-MM-dd; omit for latest
  'tlds': "com,net" // String | 
};
apiInstance.dbDroppedJson(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **date** | **Date**| yyyy-MM-dd; omit for latest | [optional] 
 **tlds** | **String**|  | [optional] 

### Return type

**[String]**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## dbExpired

> Blob dbExpired(whois, opts)

Expiring Domains

Expiring Domains. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesExpiringDroppedApi();
let whois = true; // Boolean | 
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbExpired(whois, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **whois** | **Boolean**|  | 
 **date** | **Date**| yyyy-MM-dd; omit for latest | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbExpiredCleaned

> Blob dbExpiredCleaned(opts)

Expiring Cleaned WHOIS

Expiring Cleaned WHOIS. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesExpiringDroppedApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbExpiredCleaned(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **date** | **Date**| yyyy-MM-dd; omit for latest | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


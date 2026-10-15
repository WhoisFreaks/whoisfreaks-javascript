# WhoisFreaks.DatabasesNewlyRegisteredApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbNewlyCctld**](DatabasesNewlyRegisteredApi.md#dbNewlyCctld) | **GET** /v3.1/download/domainer/cctld | Newly Registered ccTLD (CSV)
[**dbNewlyCctldCleaned**](DatabasesNewlyRegisteredApi.md#dbNewlyCctldCleaned) | **GET** /v3.1/download/domainer/cctld/cleaned | Newly Registered ccTLD Cleaned WHOIS (CSV)
[**dbNewlyCctldJson**](DatabasesNewlyRegisteredApi.md#dbNewlyCctldJson) | **GET** /v3.1/domains/newly/cctld | Newly Registered ccTLD (JSON)
[**dbNewlyDns**](DatabasesNewlyRegisteredApi.md#dbNewlyDns) | **GET** /v3.1/download/domainer/newly/dns | Newly Registered With DNS
[**dbNewlyGtld**](DatabasesNewlyRegisteredApi.md#dbNewlyGtld) | **GET** /v3.1/download/domainer/gtld | Newly Registered gTLD (CSV)
[**dbNewlyGtldCleaned**](DatabasesNewlyRegisteredApi.md#dbNewlyGtldCleaned) | **GET** /v3.1/download/domainer/gtld/cleaned | Newly Registered gTLD Cleaned WHOIS (CSV)
[**dbNewlyGtldJson**](DatabasesNewlyRegisteredApi.md#dbNewlyGtldJson) | **GET** /v3.1/domains/newly/gtld | Newly Registered gTLD (JSON)



## dbNewlyCctld

> Blob dbNewlyCctld(whois, opts)

Newly Registered ccTLD (CSV)

Newly Registered ccTLD (CSV). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let whois = true; // Boolean | 
let opts = {
  'date': new Date("2026-10-01"), // Date | yyyy-MM-dd; omit for latest
  'tlds': "com,net" // String | 
};
apiInstance.dbNewlyCctld(whois, opts).then((data) => {
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
 **tlds** | **String**|  | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbNewlyCctldCleaned

> Blob dbNewlyCctldCleaned(opts)

Newly Registered ccTLD Cleaned WHOIS (CSV)

Newly Registered ccTLD Cleaned WHOIS (CSV). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbNewlyCctldCleaned(opts).then((data) => {
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


## dbNewlyCctldJson

> [String] dbNewlyCctldJson(opts)

Newly Registered ccTLD (JSON)

Newly Registered ccTLD (JSON). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let opts = {
  'date': new Date("2026-10-01"), // Date | yyyy-MM-dd; omit for latest
  'tlds': "com,net" // String | 
};
apiInstance.dbNewlyCctldJson(opts).then((data) => {
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


## dbNewlyDns

> Blob dbNewlyDns(opts)

Newly Registered With DNS

Newly Registered With DNS. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbNewlyDns(opts).then((data) => {
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


## dbNewlyGtld

> Blob dbNewlyGtld(whois, opts)

Newly Registered gTLD (CSV)

Newly Registered gTLD (CSV). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let whois = true; // Boolean | 
let opts = {
  'date': new Date("2026-10-01"), // Date | yyyy-MM-dd; omit for latest
  'tlds': "com,net" // String | 
};
apiInstance.dbNewlyGtld(whois, opts).then((data) => {
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
 **tlds** | **String**|  | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbNewlyGtldCleaned

> Blob dbNewlyGtldCleaned(opts)

Newly Registered gTLD Cleaned WHOIS (CSV)

Newly Registered gTLD Cleaned WHOIS (CSV). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbNewlyGtldCleaned(opts).then((data) => {
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


## dbNewlyGtldJson

> [String] dbNewlyGtldJson(opts)

Newly Registered gTLD (JSON)

Newly Registered gTLD (JSON). Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesNewlyRegisteredApi();
let opts = {
  'date': new Date("2026-10-01"), // Date | yyyy-MM-dd; omit for latest
  'tlds': "com,net" // String | 
};
apiInstance.dbNewlyGtldJson(opts).then((data) => {
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


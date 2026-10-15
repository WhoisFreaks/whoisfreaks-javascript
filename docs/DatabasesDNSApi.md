# WhoisFreaks.DatabasesDNSApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbDnsDaily**](DatabasesDNSApi.md#dbDnsDaily) | **GET** /v3.2/download/dbupdate/daily/dns | DNS Database Daily
[**dbDnsMonthly**](DatabasesDNSApi.md#dbDnsMonthly) | **GET** /v3.2/download/dbupdate/monthly/dns | DNS Database Monthly
[**dbDnsWeekly**](DatabasesDNSApi.md#dbDnsWeekly) | **GET** /v3.2/download/dbupdate/weekly/dns | DNS Database Weekly



## dbDnsDaily

> Blob dbDnsDaily(opts)

DNS Database Daily

DNS Database Daily. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesDNSApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbDnsDaily(opts).then((data) => {
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


## dbDnsMonthly

> Blob dbDnsMonthly(opts)

DNS Database Monthly

DNS Database Monthly. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesDNSApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbDnsMonthly(opts).then((data) => {
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


## dbDnsWeekly

> Blob dbDnsWeekly(opts)

DNS Database Weekly

DNS Database Weekly. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesDNSApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbDnsWeekly(opts).then((data) => {
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


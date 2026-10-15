# WhoisFreaks.DatabasesSubdomainsApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbSubdomainsDaily**](DatabasesSubdomainsApi.md#dbSubdomainsDaily) | **GET** /v3.2/download/dbupdate/daily/subdomains | Subdomains Daily
[**dbSubdomainsMonthly**](DatabasesSubdomainsApi.md#dbSubdomainsMonthly) | **GET** /v3.2/download/dbupdate/monthly/subdomains | Subdomains Monthly
[**dbSubdomainsWeekly**](DatabasesSubdomainsApi.md#dbSubdomainsWeekly) | **GET** /v3.2/download/dbupdate/weekly/subdomains | Subdomains Weekly



## dbSubdomainsDaily

> Blob dbSubdomainsDaily(opts)

Subdomains Daily

Subdomains Daily. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesSubdomainsApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbSubdomainsDaily(opts).then((data) => {
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


## dbSubdomainsMonthly

> Blob dbSubdomainsMonthly(opts)

Subdomains Monthly

Subdomains Monthly. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesSubdomainsApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbSubdomainsMonthly(opts).then((data) => {
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


## dbSubdomainsWeekly

> Blob dbSubdomainsWeekly(opts)

Subdomains Weekly

Subdomains Weekly. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesSubdomainsApi();
let opts = {
  'date': new Date("2026-10-01") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbSubdomainsWeekly(opts).then((data) => {
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


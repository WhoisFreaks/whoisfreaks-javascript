# WhoisFreaks.DatabasesWHOISApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbWhoisDaily**](DatabasesWHOISApi.md#dbWhoisDaily) | **GET** /v3.3/download/dbupdate/daily/domains/whois | WHOIS Database Daily
[**dbWhoisMonthly**](DatabasesWHOISApi.md#dbWhoisMonthly) | **GET** /v3.3/download/dbupdate/monthly/domains/whois | WHOIS Database Monthly
[**dbWhoisWeekly**](DatabasesWHOISApi.md#dbWhoisWeekly) | **GET** /v3.3/download/dbupdate/weekly/domains/whois | WHOIS Database Weekly



## dbWhoisDaily

> File dbWhoisDaily(opts)

WHOIS Database Daily

WHOIS Database Daily. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesWHOISApi();
let opts = {
  'date': new Date("2013-10-20") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbWhoisDaily(opts).then((data) => {
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

**File**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbWhoisMonthly

> File dbWhoisMonthly(opts)

WHOIS Database Monthly

WHOIS Database Monthly. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesWHOISApi();
let opts = {
  'date': new Date("2013-10-20") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbWhoisMonthly(opts).then((data) => {
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

**File**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbWhoisWeekly

> File dbWhoisWeekly(opts)

WHOIS Database Weekly

WHOIS Database Weekly. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesWHOISApi();
let opts = {
  'date': new Date("2013-10-20") // Date | yyyy-MM-dd; omit for latest
};
apiInstance.dbWhoisWeekly(opts).then((data) => {
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

**File**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


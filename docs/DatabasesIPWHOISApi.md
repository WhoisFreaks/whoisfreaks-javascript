# WhoisFreaks.DatabasesIPWHOISApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbIpWhois**](DatabasesIPWHOISApi.md#dbIpWhois) | **GET** /v3.3/download/snapshot/ip/whois | IP WHOIS Snapshot
[**dbIpWhoisStatus**](DatabasesIPWHOISApi.md#dbIpWhoisStatus) | **GET** /v3.3/status/snapshot/ip/whois | IP WHOIS Snapshot Status



## dbIpWhois

> File dbIpWhois(date)

IP WHOIS Snapshot

IP WHOIS Snapshot. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesIPWHOISApi();
let date = new Date("2013-10-20"); // Date | 
apiInstance.dbIpWhois(date).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **date** | **Date**|  | 

### Return type

**File**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## dbIpWhoisStatus

> SnapshotStatus dbIpWhoisStatus()

IP WHOIS Snapshot Status

IP WHOIS Snapshot Status. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesIPWHOISApi();
apiInstance.dbIpWhoisStatus().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

[**SnapshotStatus**](SnapshotStatus.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


# WhoisFreaks.DatabasesASNWHOISApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dbAsnWhois**](DatabasesASNWHOISApi.md#dbAsnWhois) | **GET** /v3.3/download/snapshot/asn/whois | ASN WHOIS Snapshot
[**dbAsnWhoisStatus**](DatabasesASNWHOISApi.md#dbAsnWhoisStatus) | **GET** /v3.3/status/snapshot/asn/whois | ASN WHOIS Snapshot Status



## dbAsnWhois

> File dbAsnWhois(date)

ASN WHOIS Snapshot

ASN WHOIS Snapshot. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesASNWHOISApi();
let date = new Date("2013-10-20"); // Date | 
apiInstance.dbAsnWhois(date).then((data) => {
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


## dbAsnWhoisStatus

> SnapshotStatus dbAsnWhoisStatus()

ASN WHOIS Snapshot Status

ASN WHOIS Snapshot Status. Returns the file/snapshot described by this operation.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesASNWHOISApi();
apiInstance.dbAsnWhoisStatus().then((data) => {
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


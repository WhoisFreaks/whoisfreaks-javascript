# WhoisFreaks.DatabasesThreatFeedApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**downloadThreatFeedMalware**](DatabasesThreatFeedApi.md#downloadThreatFeedMalware) | **GET** /v3.4/download/threat-feed/malware | Download the daily malware threat feed (CSV)
[**downloadThreatFeedMalwareSample**](DatabasesThreatFeedApi.md#downloadThreatFeedMalwareSample) | **GET** /v3.4/download/threat-feed/malware/sample | Download a sample of the malware threat feed (CSV)
[**downloadThreatFeedPhishing**](DatabasesThreatFeedApi.md#downloadThreatFeedPhishing) | **GET** /v3.4/download/threat-feed/phishing | Download the daily phishing threat feed (CSV)
[**downloadThreatFeedPhishingSample**](DatabasesThreatFeedApi.md#downloadThreatFeedPhishingSample) | **GET** /v3.4/download/threat-feed/phishing/sample | Download a sample of the phishing threat feed (CSV)
[**downloadThreatFeedSpam**](DatabasesThreatFeedApi.md#downloadThreatFeedSpam) | **GET** /v3.4/download/threat-feed/spam | Download the daily spam threat feed (CSV)
[**downloadThreatFeedSpamSample**](DatabasesThreatFeedApi.md#downloadThreatFeedSpamSample) | **GET** /v3.4/download/threat-feed/spam/sample | Download a sample of the spam threat feed (CSV)



## downloadThreatFeedMalware

> Blob downloadThreatFeedMalware(opts)

Download the daily malware threat feed (CSV)

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesThreatFeedApi();
let opts = {
  'date': "2026-10-01" // String | Feed date (yyyy-MM-dd); omit for the full dump of the feed
};
apiInstance.downloadThreatFeedMalware(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **date** | **String**| Feed date (yyyy-MM-dd); omit for the full dump of the feed | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## downloadThreatFeedMalwareSample

> Blob downloadThreatFeedMalwareSample()

Download a sample of the malware threat feed (CSV)

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesThreatFeedApi();
apiInstance.downloadThreatFeedMalwareSample().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## downloadThreatFeedPhishing

> Blob downloadThreatFeedPhishing(opts)

Download the daily phishing threat feed (CSV)

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesThreatFeedApi();
let opts = {
  'date': "2026-10-01" // String | Feed date (yyyy-MM-dd); omit for the full dump of the feed
};
apiInstance.downloadThreatFeedPhishing(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **date** | **String**| Feed date (yyyy-MM-dd); omit for the full dump of the feed | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## downloadThreatFeedPhishingSample

> Blob downloadThreatFeedPhishingSample()

Download a sample of the phishing threat feed (CSV)

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesThreatFeedApi();
apiInstance.downloadThreatFeedPhishingSample().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## downloadThreatFeedSpam

> Blob downloadThreatFeedSpam(opts)

Download the daily spam threat feed (CSV)

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesThreatFeedApi();
let opts = {
  'date': "2026-10-01" // String | Feed date (yyyy-MM-dd); omit for the full dump of the feed
};
apiInstance.downloadThreatFeedSpam(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **date** | **String**| Feed date (yyyy-MM-dd); omit for the full dump of the feed | [optional] 

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


## downloadThreatFeedSpamSample

> Blob downloadThreatFeedSpamSample()

Download a sample of the spam threat feed (CSV)

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DatabasesThreatFeedApi();
apiInstance.downloadThreatFeedSpamSample().then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters

This endpoint does not need any parameter.

### Return type

**Blob**

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/octet-stream, application/json


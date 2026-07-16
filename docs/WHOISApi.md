# WhoisFreaks.WHOISApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulkWhois**](WHOISApi.md#bulkWhois) | **POST** /v2.0/bulkwhois/live | Bulk WHOIS Lookup
[**whoisHistory**](WHOISApi.md#whoisHistory) | **GET** /v2.0/whois/history | Historical WHOIS records for a domain
[**whoisLive**](WHOISApi.md#whoisLive) | **GET** /v2.0/whois/live | Live WHOIS Lookup
[**whoisReverse**](WHOISApi.md#whoisReverse) | **GET** /v2.0/whois/reverse | Reverse WHOIS lookup by keyword



## bulkWhois

> BulkWhoisResponse bulkWhois(bulkWhoisRequest, opts)

Bulk WHOIS Lookup

Up to 100 domains in one request. 1 credit per successful domain.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.WHOISApi();
let bulkWhoisRequest = new WhoisFreaks.BulkWhoisRequest(); // BulkWhoisRequest | 
let opts = {
  'format': "'json'" // String | 
};
apiInstance.bulkWhois(bulkWhoisRequest, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkWhoisRequest** | [**BulkWhoisRequest**](BulkWhoisRequest.md)|  | 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**BulkWhoisResponse**](BulkWhoisResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## whoisHistory

> WhoisHistoricalResponse whoisHistory(domainName, opts)

Historical WHOIS records for a domain

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.WHOISApi();
let domainName = "domainName_example"; // String | Domain to fetch historical WHOIS records for
let opts = {
  'page': 56, // Number | Page number
  'format': "format_example" // String | 
};
apiInstance.whoisHistory(domainName, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domainName** | **String**| Domain to fetch historical WHOIS records for | 
 **page** | **Number**| Page number | [optional] 
 **format** | **String**|  | [optional] 

### Return type

[**WhoisHistoricalResponse**](WhoisHistoricalResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## whoisLive

> WhoisResponse whoisLive(domainName, opts)

Live WHOIS Lookup

Real-time WHOIS lookup from authoritative servers. Cost 1 credit.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.WHOISApi();
let domainName = "whoisfreaks.com"; // String | 
let opts = {
  'format': "'json'" // String | 
};
apiInstance.whoisLive(domainName, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domainName** | **String**|  | 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**WhoisResponse**](WhoisResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## whoisReverse

> ReverseWhoisResponse whoisReverse(keyword, opts)

Reverse WHOIS lookup by keyword

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.WHOISApi();
let keyword = "keyword_example"; // String | Keyword to search across WHOIS records
let opts = {
  'page': 56, // Number | Page number
  'format': "format_example" // String | 
};
apiInstance.whoisReverse(keyword, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyword** | **String**| Keyword to search across WHOIS records | 
 **page** | **Number**| Page number | [optional] 
 **format** | **String**|  | [optional] 

### Return type

[**ReverseWhoisResponse**](ReverseWhoisResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


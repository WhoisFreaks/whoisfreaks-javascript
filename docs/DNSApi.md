# WhoisFreaks.DNSApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**dnsBulk**](DNSApi.md#dnsBulk) | **POST** /v2.0/dns/bulk/live | Bulk DNS Lookup
[**dnsHistorical**](DNSApi.md#dnsHistorical) | **GET** /v2.0/dns/historical | Historical DNS Lookup
[**dnsLive**](DNSApi.md#dnsLive) | **GET** /v2.0/dns/live | Live DNS Lookup
[**dnsReverse**](DNSApi.md#dnsReverse) | **GET** /v2.1/dns/reverse | Reverse DNS Lookup



## dnsBulk

> BulkDnsResponse dnsBulk(type, dnsBulkRequest, opts)

Bulk DNS Lookup

Up to 100 domains + 100 IPs in one request.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DNSApi();
let type = "A,MX,TXT"; // String | 
let dnsBulkRequest = new WhoisFreaks.DnsBulkRequest(); // DnsBulkRequest | 
let opts = {
  'format': "'json'" // String | 
};
apiInstance.dnsBulk(type, dnsBulkRequest, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **String**|  | [default to &#39;all&#39;]
 **dnsBulkRequest** | [**DnsBulkRequest**](DnsBulkRequest.md)|  | 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**BulkDnsResponse**](BulkDnsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## dnsHistorical

> HistoricalDnsResponse dnsHistorical(domainName, type, opts)

Historical DNS Lookup

All historical DNS records. 2 credits per page (100 records/page).

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DNSApi();
let domainName = "whoisfreaks.com"; // String | 
let type = "A,MX,TXT"; // String | 
let opts = {
  'page': 1, // Number | 
  'format': "'json'" // String | 
};
apiInstance.dnsHistorical(domainName, type, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domainName** | **String**|  | 
 **type** | **String**|  | [default to &#39;all&#39;]
 **page** | **Number**|  | [optional] [default to 1]
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**HistoricalDnsResponse**](HistoricalDnsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## dnsLive

> DnsResponse dnsLive(type, opts)

Live DNS Lookup

Real-time DNS record lookup. 1 credit per query.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DNSApi();
let type = "A,MX,TXT"; // String | all or comma-separated: A,MX,NS,TXT,SOA,SPF,AAAA,CNAME
let opts = {
  'domainName': "whoisfreaks.com", // String | 
  'ipAddress': "8.8.8.8", // String | Use for PTR lookups
  'format': "'json'" // String | 
};
apiInstance.dnsLive(type, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **type** | **String**| all or comma-separated: A,MX,NS,TXT,SOA,SPF,AAAA,CNAME | [default to &#39;all&#39;]
 **domainName** | **String**|  | [optional] 
 **ipAddress** | **String**| Use for PTR lookups | [optional] 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**DnsResponse**](DnsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## dnsReverse

> ReverseDnsResponse dnsReverse(value, type, opts)

Reverse DNS Lookup

Search domains by IP or DNS value. 5 credits per page.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DNSApi();
let value = "8.8.8.8"; // String | IP, CIDR, or record value
let type = "type_example"; // String | 
let opts = {
  'exact': true, // Boolean | 
  'page': 1, // Number | 
  'format': "'json'" // String | 
};
apiInstance.dnsReverse(value, type, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **value** | **String**| IP, CIDR, or record value | 
 **type** | **String**|  | 
 **exact** | **Boolean**|  | [optional] [default to true]
 **page** | **Number**|  | [optional] [default to 1]
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**ReverseDnsResponse**](ReverseDnsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


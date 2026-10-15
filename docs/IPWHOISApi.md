# WhoisFreaks.IPWHOISApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ipWhois**](IPWHOISApi.md#ipWhois) | **GET** /v1.0/ip-whois | IP WHOIS Lookup



## ipWhois

> IpWhoisResponse ipWhois(ip, opts)

IP WHOIS Lookup

WHOIS for an IP address. 1 credit.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.IPWHOISApi();
let ip = "8.8.8.8"; // String | 
let opts = {
  'format': "'json'" // String | 
};
apiInstance.ipWhois(ip, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ip** | **String**|  | 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**IpWhoisResponse**](IpWhoisResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


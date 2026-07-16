# WhoisFreaks.SubdomainsApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**subdomains**](SubdomainsApi.md#subdomains) | **GET** /v1.0/subdomains | Subdomains Lookup



## subdomains

> SubdomainsResponse subdomains(domain, opts)

Subdomains Lookup

All subdomains including nested. 2 credits per query.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.SubdomainsApi();
let domain = "domain_example"; // String | 
let opts = {
  'after': new Date("2013-10-20"), // Date | 
  'before': new Date("2013-10-20"), // Date | 
  'status': "status_example", // String | 
  'page': 1, // Number | 
  'format': "'json'" // String | 
};
apiInstance.subdomains(domain, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**|  | 
 **after** | **Date**|  | [optional] 
 **before** | **Date**|  | [optional] 
 **status** | **String**|  | [optional] 
 **page** | **Number**|  | [optional] [default to 1]
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**SubdomainsResponse**](SubdomainsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


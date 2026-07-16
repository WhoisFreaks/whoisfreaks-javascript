# WhoisFreaks.SSLApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**sslLookup**](SSLApi.md#sslLookup) | **GET** /v1.0/ssl/live | SSL Certificate Lookup



## sslLookup

> SslResponse sslLookup(domainName, opts)

SSL Certificate Lookup

Real-time SSL cert with optional chain.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.SSLApi();
let domainName = "domainName_example"; // String | 
let opts = {
  'chain': false, // Boolean | 
  'sslRaw': false, // Boolean | 
  'format': "'json'" // String | 
};
apiInstance.sslLookup(domainName, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domainName** | **String**|  | 
 **chain** | **Boolean**|  | [optional] [default to false]
 **sslRaw** | **Boolean**|  | [optional] [default to false]
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**SslResponse**](SslResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


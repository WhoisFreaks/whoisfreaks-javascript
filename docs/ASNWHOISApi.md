# WhoisFreaks.ASNWHOISApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**asnWhois**](ASNWHOISApi.md#asnWhois) | **GET** /v2.0/asn-whois | ASN WHOIS Lookup



## asnWhois

> AsnWhoisResponse asnWhois(asn, opts)

ASN WHOIS Lookup

WHOIS for an ASN. 1 credit.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.ASNWHOISApi();
let asn = "as15169"; // String | 
let opts = {
  'format': "'json'" // String | 
};
apiInstance.asnWhois(asn, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **asn** | **String**|  | 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**AsnWhoisResponse**](AsnWhoisResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


# WhoisFreaks.TyposquattingApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**typosquatting**](TyposquattingApi.md#typosquatting) | **GET** /v3.0/domain/typos | Typosquatting Lookup



## typosquatting

> TyposquattingResponse typosquatting(opts)

Typosquatting Lookup

Find typo variants of a brand. 5 credits per page.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.TyposquattingApi();
let opts = {
  'keyword': "whoisfreaks", // String | 
  'pattern': "whois*", // String | 
  'pageToken': "pageToken_example" // String | 
};
apiInstance.typosquatting(opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **keyword** | **String**|  | [optional] 
 **pattern** | **String**|  | [optional] 
 **pageToken** | **String**|  | [optional] 

### Return type

[**TyposquattingResponse**](TyposquattingResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


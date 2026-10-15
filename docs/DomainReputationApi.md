# WhoisFreaks.DomainReputationApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**domainReputation**](DomainReputationApi.md#domainReputation) | **GET** /v1/domain/security | Domain Reputation Lookup



## domainReputation

> DomainReputationResponse domainReputation(domainName, opts)

Domain Reputation Lookup

Real-time domain threat assessment. Returns risk verdict, trust score, DGA analysis, threat intelligence matches, and security signals. 1 credit.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks-js';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DomainReputationApi();
let domainName = "amazon.com"; // String | The domain name to assess
let opts = {
  'format': "'json'" // String | 
};
apiInstance.domainReputation(domainName, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domainName** | **String**| The domain name to assess | 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**DomainReputationResponse**](DomainReputationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


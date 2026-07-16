# WhoisFreaks.DomainAvailabilityApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulkDomainAvailabilityV2**](DomainAvailabilityApi.md#bulkDomainAvailabilityV2) | **POST** /v2.0/domain/availability | Bulk Domain Availability Check
[**domainAvailabilityV2**](DomainAvailabilityApi.md#domainAvailabilityV2) | **GET** /v2.0/domain/availability | Domain Availability Check with Suggestions



## bulkDomainAvailabilityV2

> BulkDomainAvailabilityResponse bulkDomainAvailabilityV2(bulkDomainAvailabilityRequest, opts)

Bulk Domain Availability Check

Two bulk modes. Mode 1: POST domainNames array. Mode 2: POST tld array plus domain query param. Max 100 domains per request. 1 credit per domain checked.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DomainAvailabilityApi();
let bulkDomainAvailabilityRequest = new WhoisFreaks.BulkDomainAvailabilityRequest(); // BulkDomainAvailabilityRequest | 
let opts = {
  'domain': "google.com", // String | Required for TLD-mode bulk check (base domain).
  'format': "'json'" // String | 
};
apiInstance.bulkDomainAvailabilityV2(bulkDomainAvailabilityRequest, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkDomainAvailabilityRequest** | [**BulkDomainAvailabilityRequest**](BulkDomainAvailabilityRequest.md)|  | 
 **domain** | **String**| Required for TLD-mode bulk check (base domain). | [optional] 
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**BulkDomainAvailabilityResponse**](BulkDomainAvailabilityResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## domainAvailabilityV2

> DomainAvailabilityResponse domainAvailabilityV2(domain, opts)

Domain Availability Check with Suggestions

Check availability of a single domain and optionally get suggestions across multiple TLDs. 1 credit per domain checked. sug&#x3D;false checks only the queried domain; sug&#x3D;true returns up to &#x60;count&#x60; (max 100) TLD suggestions.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.DomainAvailabilityApi();
let domain = "google.com"; // String | The domain name to check
let opts = {
  'sug': false, // Boolean | Whether to return TLD suggestions alongside the queried domain.
  'count': 5, // Number | Number of TLD suggestions to return when sug=true. Maximum is 100.
  'format': "'json'" // String | 
};
apiInstance.domainAvailabilityV2(domain, opts).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **domain** | **String**| The domain name to check | 
 **sug** | **Boolean**| Whether to return TLD suggestions alongside the queried domain. | [optional] [default to false]
 **count** | **Number**| Number of TLD suggestions to return when sug&#x3D;true. Maximum is 100. | [optional] [default to 5]
 **format** | **String**|  | [optional] [default to &#39;json&#39;]

### Return type

[**DomainAvailabilityResponse**](DomainAvailabilityResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


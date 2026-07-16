# WhoisFreaks.IPReputationApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulkIpReputation**](IPReputationApi.md#bulkIpReputation) | **POST** /v1.0/security | Bulk IP Reputation
[**ipReputation**](IPReputationApi.md#ipReputation) | **GET** /v1.0/security | IP Reputation Lookup



## bulkIpReputation

> [IpReputationResponse] bulkIpReputation(bulkGeolocationRequest)

Bulk IP Reputation

Up to 100 IPs.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.IPReputationApi();
let bulkGeolocationRequest = new WhoisFreaks.BulkGeolocationRequest(); // BulkGeolocationRequest | 
apiInstance.bulkIpReputation(bulkGeolocationRequest).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bulkGeolocationRequest** | [**BulkGeolocationRequest**](BulkGeolocationRequest.md)|  | 

### Return type

[**[IpReputationResponse]**](IpReputationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## ipReputation

> IpReputationResponse ipReputation(ip)

IP Reputation Lookup

Threat intel for IP — VPN, proxy, Tor, bots. 1 credit.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.IPReputationApi();
let ip = "ip_example"; // String | 
apiInstance.ipReputation(ip).then((data) => {
  console.log('API called successfully. Returned data: ' + data);
}, (error) => {
  console.error(error);
});

```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ip** | **String**|  | 

### Return type

[**IpReputationResponse**](IpReputationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


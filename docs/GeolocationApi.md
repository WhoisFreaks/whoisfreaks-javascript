# WhoisFreaks.GeolocationApi

All URIs are relative to *https://api.whoisfreaks.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bulkGeolocation**](GeolocationApi.md#bulkGeolocation) | **POST** /v1.0/geolocation | Bulk IP Geolocation
[**geolocation**](GeolocationApi.md#geolocation) | **GET** /v1.0/geolocation | IP Geolocation Lookup



## bulkGeolocation

> [GeolocationResponse] bulkGeolocation(bulkGeolocationRequest)

Bulk IP Geolocation

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

let apiInstance = new WhoisFreaks.GeolocationApi();
let bulkGeolocationRequest = new WhoisFreaks.BulkGeolocationRequest(); // BulkGeolocationRequest | 
apiInstance.bulkGeolocation(bulkGeolocationRequest).then((data) => {
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

[**[GeolocationResponse]**](GeolocationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## geolocation

> GeolocationResponse geolocation(ip)

IP Geolocation Lookup

Get location, ASN, currency for an IP. 1 credit.

### Example

```javascript
import WhoisFreaks from 'whoisfreaks';
let defaultClient = WhoisFreaks.ApiClient.instance;
// Configure API key authorization: ApiKeyAuth
let ApiKeyAuth = defaultClient.authentications['ApiKeyAuth'];
ApiKeyAuth.apiKey = 'YOUR API KEY';
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//ApiKeyAuth.apiKeyPrefix = 'Token';

let apiInstance = new WhoisFreaks.GeolocationApi();
let ip = "ip_example"; // String | 
apiInstance.geolocation(ip).then((data) => {
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

[**GeolocationResponse**](GeolocationResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


# RagsearchesApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost**](RagsearchesApi.md#createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost) | **POST** /v3/rag/searches/reference_objects | Create A Reference Object Search

<a name="createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost"></a>
# **createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost**
> CreateReferenceObjectSearchResponseModel createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost(body, corpusId)

Create A Reference Object Search

Creates a reference object search query and returns results.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagsearchesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagsearchesApi apiInstance = new RagsearchesApi();
CreateReferenceObjectSearchRequestModel body = new CreateReferenceObjectSearchRequestModel(); // CreateReferenceObjectSearchRequestModel | 
Object corpusId = null; // Object | 
try {
    CreateReferenceObjectSearchResponseModel result = apiInstance.createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost(body, corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagsearchesApi#createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateReferenceObjectSearchRequestModel**](CreateReferenceObjectSearchRequestModel.md)|  |
 **corpusId** | [**Object**](.md)|  | [optional]

### Return type

[**CreateReferenceObjectSearchResponseModel**](CreateReferenceObjectSearchResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


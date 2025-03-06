# RagreferenceObjectsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createsAReferenceObjectV3RagReferenceObjectsPost**](RagreferenceObjectsApi.md#createsAReferenceObjectV3RagReferenceObjectsPost) | **POST** /v3/rag/reference_objects | Creates A Reference Object
[**deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete**](RagreferenceObjectsApi.md#deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete) | **DELETE** /v3/rag/reference_objects/{reference_object_id} | Deletes A Reference Object
[**getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet**](RagreferenceObjectsApi.md#getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet) | **GET** /v3/rag/reference_objects/{reference_object_id} | Get A Reference Object
[**listsAllReferenceObjectsV3RagReferenceObjectsGet**](RagreferenceObjectsApi.md#listsAllReferenceObjectsV3RagReferenceObjectsGet) | **GET** /v3/rag/reference_objects | Lists All Reference Objects

<a name="createsAReferenceObjectV3RagReferenceObjectsPost"></a>
# **createsAReferenceObjectV3RagReferenceObjectsPost**
> CreateReferenceObjectResponseModel createsAReferenceObjectV3RagReferenceObjectsPost(uploadFile, corpusId)

Creates A Reference Object

Creates an reference object.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagreferenceObjectsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagreferenceObjectsApi apiInstance = new RagreferenceObjectsApi();
Object uploadFile = null; // Object | 
Object corpusId = null; // Object | 
try {
    CreateReferenceObjectResponseModel result = apiInstance.createsAReferenceObjectV3RagReferenceObjectsPost(uploadFile, corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagreferenceObjectsApi#createsAReferenceObjectV3RagReferenceObjectsPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **uploadFile** | [**Object**](.md)|  |
 **corpusId** | [**Object**](.md)|  |

### Return type

[**CreateReferenceObjectResponseModel**](CreateReferenceObjectResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: multipart/form-data
 - **Accept**: application/json

<a name="deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete"></a>
# **deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete**
> DeleteReferenceObjectResponseModel deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete(referenceObjectId)

Deletes A Reference Object

Deletes the reference object specified in &#x60;reference_object_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagreferenceObjectsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagreferenceObjectsApi apiInstance = new RagreferenceObjectsApi();
Object referenceObjectId = null; // Object | 
try {
    DeleteReferenceObjectResponseModel result = apiInstance.deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete(referenceObjectId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagreferenceObjectsApi#deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **referenceObjectId** | [**Object**](.md)|  |

### Return type

[**DeleteReferenceObjectResponseModel**](DeleteReferenceObjectResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet"></a>
# **getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet**
> GetReferenceObjectResponseModel getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet(referenceObjectId)

Get A Reference Object

Returns a reference object matching the provided &#x60;reference_object_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagreferenceObjectsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagreferenceObjectsApi apiInstance = new RagreferenceObjectsApi();
Object referenceObjectId = null; // Object | 
try {
    GetReferenceObjectResponseModel result = apiInstance.getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet(referenceObjectId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagreferenceObjectsApi#getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **referenceObjectId** | [**Object**](.md)|  |

### Return type

[**GetReferenceObjectResponseModel**](GetReferenceObjectResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listsAllReferenceObjectsV3RagReferenceObjectsGet"></a>
# **listsAllReferenceObjectsV3RagReferenceObjectsGet**
> ListReferenceObjectsResponseModel listsAllReferenceObjectsV3RagReferenceObjectsGet()

Lists All Reference Objects

Lists all corpora.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagreferenceObjectsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagreferenceObjectsApi apiInstance = new RagreferenceObjectsApi();
try {
    ListReferenceObjectsResponseModel result = apiInstance.listsAllReferenceObjectsV3RagReferenceObjectsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagreferenceObjectsApi#listsAllReferenceObjectsV3RagReferenceObjectsGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListReferenceObjectsResponseModel**](ListReferenceObjectsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


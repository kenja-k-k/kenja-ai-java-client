# RagApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createACorpusV3RagCorporaPost**](RagApi.md#createACorpusV3RagCorporaPost) | **POST** /v3/rag/corpora | Create A Corpus
[**createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost**](RagApi.md#createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost) | **POST** /v3/rag/searches/reference_objects | Create A Reference Object Search
[**createsAReferenceObjectV3RagReferenceObjectsPost**](RagApi.md#createsAReferenceObjectV3RagReferenceObjectsPost) | **POST** /v3/rag/reference_objects | Creates A Reference Object
[**deleteACorpusV3RagCorporaCorpusIdDelete**](RagApi.md#deleteACorpusV3RagCorporaCorpusIdDelete) | **DELETE** /v3/rag/corpora/{corpus_id} | Delete A Corpus
[**deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete**](RagApi.md#deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete) | **DELETE** /v3/rag/reference_objects/{reference_object_id} | Deletes A Reference Object
[**getACorpusV3RagCorporaCorpusIdGet**](RagApi.md#getACorpusV3RagCorporaCorpusIdGet) | **GET** /v3/rag/corpora/{corpus_id} | Get A Corpus
[**getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet**](RagApi.md#getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet) | **GET** /v3/rag/reference_objects/{reference_object_id} | Get A Reference Object
[**listAllCorporaV3RagCorporaGet**](RagApi.md#listAllCorporaV3RagCorporaGet) | **GET** /v3/rag/corpora | List All Corpora
[**listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet**](RagApi.md#listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet) | **GET** /v3/rag/corpora/{corpus_id}/reference_objects | List Corpus Reference Objects
[**listsAllReferenceObjectsV3RagReferenceObjectsGet**](RagApi.md#listsAllReferenceObjectsV3RagReferenceObjectsGet) | **GET** /v3/rag/reference_objects | Lists All Reference Objects
[**updateACorpusV3RagCorporaCorpusIdPatch**](RagApi.md#updateACorpusV3RagCorporaCorpusIdPatch) | **PATCH** /v3/rag/corpora/{corpus_id} | Update A Corpus

<a name="createACorpusV3RagCorporaPost"></a>
# **createACorpusV3RagCorporaPost**
> CreateCorpusResponseModel createACorpusV3RagCorporaPost(body)

Create A Corpus

Creates a corpus.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
CreateCorpusRequestModel body = new CreateCorpusRequestModel(); // CreateCorpusRequestModel | 
try {
    CreateCorpusResponseModel result = apiInstance.createACorpusV3RagCorporaPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#createACorpusV3RagCorporaPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateCorpusRequestModel**](CreateCorpusRequestModel.md)|  |

### Return type

[**CreateCorpusResponseModel**](CreateCorpusResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

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
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
CreateReferenceObjectSearchRequestModel body = new CreateReferenceObjectSearchRequestModel(); // CreateReferenceObjectSearchRequestModel | 
Object corpusId = null; // Object | 
try {
    CreateReferenceObjectSearchResponseModel result = apiInstance.createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost(body, corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#createAReferenceObjectSearchV3RagSearchesReferenceObjectsPost");
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
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
Object uploadFile = null; // Object | 
Object corpusId = null; // Object | 
try {
    CreateReferenceObjectResponseModel result = apiInstance.createsAReferenceObjectV3RagReferenceObjectsPost(uploadFile, corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#createsAReferenceObjectV3RagReferenceObjectsPost");
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

<a name="deleteACorpusV3RagCorporaCorpusIdDelete"></a>
# **deleteACorpusV3RagCorporaCorpusIdDelete**
> DeleteCorpusResponseModel deleteACorpusV3RagCorporaCorpusIdDelete(corpusId)

Delete A Corpus

Deletes the corpus specified in &#x60;corpus_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
Object corpusId = null; // Object | 
try {
    DeleteCorpusResponseModel result = apiInstance.deleteACorpusV3RagCorporaCorpusIdDelete(corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#deleteACorpusV3RagCorporaCorpusIdDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **corpusId** | [**Object**](.md)|  |

### Return type

[**DeleteCorpusResponseModel**](DeleteCorpusResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
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
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
Object referenceObjectId = null; // Object | 
try {
    DeleteReferenceObjectResponseModel result = apiInstance.deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete(referenceObjectId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#deletesAReferenceObjectV3RagReferenceObjectsReferenceObjectIdDelete");
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

<a name="getACorpusV3RagCorporaCorpusIdGet"></a>
# **getACorpusV3RagCorporaCorpusIdGet**
> GetCorpusResponseModel getACorpusV3RagCorporaCorpusIdGet(corpusId)

Get A Corpus

Returns a corpus matching the provided &#x60;corpus_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
Object corpusId = null; // Object | 
try {
    GetCorpusResponseModel result = apiInstance.getACorpusV3RagCorporaCorpusIdGet(corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#getACorpusV3RagCorporaCorpusIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **corpusId** | [**Object**](.md)|  |

### Return type

[**GetCorpusResponseModel**](GetCorpusResponseModel.md)

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
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
Object referenceObjectId = null; // Object | 
try {
    GetReferenceObjectResponseModel result = apiInstance.getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet(referenceObjectId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#getAReferenceObjectV3RagReferenceObjectsReferenceObjectIdGet");
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

<a name="listAllCorporaV3RagCorporaGet"></a>
# **listAllCorporaV3RagCorporaGet**
> ListCorporaResponseModel listAllCorporaV3RagCorporaGet()

List All Corpora

Lists all corpora.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
try {
    ListCorporaResponseModel result = apiInstance.listAllCorporaV3RagCorporaGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#listAllCorporaV3RagCorporaGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListCorporaResponseModel**](ListCorporaResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet"></a>
# **listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet**
> ListCorpusReferenceObjectsResponseModel listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet(corpusId)

List Corpus Reference Objects

Lists all reference objects associated with a corpus specified in &#x60;organization_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
Object corpusId = null; // Object | 
try {
    ListCorpusReferenceObjectsResponseModel result = apiInstance.listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet(corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **corpusId** | [**Object**](.md)|  |

### Return type

[**ListCorpusReferenceObjectsResponseModel**](ListCorpusReferenceObjectsResponseModel.md)

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
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
try {
    ListReferenceObjectsResponseModel result = apiInstance.listsAllReferenceObjectsV3RagReferenceObjectsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#listsAllReferenceObjectsV3RagReferenceObjectsGet");
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

<a name="updateACorpusV3RagCorporaCorpusIdPatch"></a>
# **updateACorpusV3RagCorporaCorpusIdPatch**
> UpdateCorpusResponseModel updateACorpusV3RagCorporaCorpusIdPatch(body, corpusId)

Update A Corpus

Updates the corpus specified in &#x60;corpus_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.RagApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagApi apiInstance = new RagApi();
UpdateCorpusRequestModel body = new UpdateCorpusRequestModel(); // UpdateCorpusRequestModel | 
Object corpusId = null; // Object | 
try {
    UpdateCorpusResponseModel result = apiInstance.updateACorpusV3RagCorporaCorpusIdPatch(body, corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagApi#updateACorpusV3RagCorporaCorpusIdPatch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateCorpusRequestModel**](UpdateCorpusRequestModel.md)|  |
 **corpusId** | [**Object**](.md)|  |

### Return type

[**UpdateCorpusResponseModel**](UpdateCorpusResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


# RagcorporaApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createACorpusV3RagCorporaPost**](RagcorporaApi.md#createACorpusV3RagCorporaPost) | **POST** /v3/rag/corpora | Create A Corpus
[**deleteACorpusV3RagCorporaCorpusIdDelete**](RagcorporaApi.md#deleteACorpusV3RagCorporaCorpusIdDelete) | **DELETE** /v3/rag/corpora/{corpus_id} | Delete A Corpus
[**getACorpusV3RagCorporaCorpusIdGet**](RagcorporaApi.md#getACorpusV3RagCorporaCorpusIdGet) | **GET** /v3/rag/corpora/{corpus_id} | Get A Corpus
[**listAllCorporaV3RagCorporaGet**](RagcorporaApi.md#listAllCorporaV3RagCorporaGet) | **GET** /v3/rag/corpora | List All Corpora
[**listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet**](RagcorporaApi.md#listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet) | **GET** /v3/rag/corpora/{corpus_id}/reference_objects | List Corpus Reference Objects
[**updateACorpusV3RagCorporaCorpusIdPatch**](RagcorporaApi.md#updateACorpusV3RagCorporaCorpusIdPatch) | **PATCH** /v3/rag/corpora/{corpus_id} | Update A Corpus

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
//import io.swagger.client.api.RagcorporaApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagcorporaApi apiInstance = new RagcorporaApi();
CreateCorpusRequestModel body = new CreateCorpusRequestModel(); // CreateCorpusRequestModel | 
try {
    CreateCorpusResponseModel result = apiInstance.createACorpusV3RagCorporaPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagcorporaApi#createACorpusV3RagCorporaPost");
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
//import io.swagger.client.api.RagcorporaApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagcorporaApi apiInstance = new RagcorporaApi();
Object corpusId = null; // Object | 
try {
    DeleteCorpusResponseModel result = apiInstance.deleteACorpusV3RagCorporaCorpusIdDelete(corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagcorporaApi#deleteACorpusV3RagCorporaCorpusIdDelete");
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
//import io.swagger.client.api.RagcorporaApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagcorporaApi apiInstance = new RagcorporaApi();
Object corpusId = null; // Object | 
try {
    GetCorpusResponseModel result = apiInstance.getACorpusV3RagCorporaCorpusIdGet(corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagcorporaApi#getACorpusV3RagCorporaCorpusIdGet");
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
//import io.swagger.client.api.RagcorporaApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagcorporaApi apiInstance = new RagcorporaApi();
try {
    ListCorporaResponseModel result = apiInstance.listAllCorporaV3RagCorporaGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagcorporaApi#listAllCorporaV3RagCorporaGet");
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
//import io.swagger.client.api.RagcorporaApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagcorporaApi apiInstance = new RagcorporaApi();
Object corpusId = null; // Object | 
try {
    ListCorpusReferenceObjectsResponseModel result = apiInstance.listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet(corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagcorporaApi#listCorpusReferenceObjectsV3RagCorporaCorpusIdReferenceObjectsGet");
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
//import io.swagger.client.api.RagcorporaApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


RagcorporaApi apiInstance = new RagcorporaApi();
UpdateCorpusRequestModel body = new UpdateCorpusRequestModel(); // UpdateCorpusRequestModel | 
Object corpusId = null; // Object | 
try {
    UpdateCorpusResponseModel result = apiInstance.updateACorpusV3RagCorporaCorpusIdPatch(body, corpusId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RagcorporaApi#updateACorpusV3RagCorporaCorpusIdPatch");
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


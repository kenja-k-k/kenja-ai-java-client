# ModelsembeddingsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet**](ModelsembeddingsApi.md#listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet) | **GET** /v3/models/embeddings | List All Embedding Inference Providers
[**listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet**](ModelsembeddingsApi.md#listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet) | **GET** /v3/models/embeddings/{embedding_inference_provider_id} | List Embedding Inference Provider Models

<a name="listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet"></a>
# **listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet**
> ListEmbeddingInferenceProvidersResponseModel listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet()

List All Embedding Inference Providers

List all embedding inference providers.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsembeddingsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsembeddingsApi apiInstance = new ModelsembeddingsApi();
try {
    ListEmbeddingInferenceProvidersResponseModel result = apiInstance.listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsembeddingsApi#listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListEmbeddingInferenceProvidersResponseModel**](ListEmbeddingInferenceProvidersResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet"></a>
# **listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet**
> ListEmbeddingInferenceProviderModelsResponseModel listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet(embeddingInferenceProviderId)

List Embedding Inference Provider Models

Lists all embedding models in the provided embedding inference provider.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsembeddingsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsembeddingsApi apiInstance = new ModelsembeddingsApi();
EmbeddingInferenceProviderID embeddingInferenceProviderId = new EmbeddingInferenceProviderID(); // EmbeddingInferenceProviderID | 
try {
    ListEmbeddingInferenceProviderModelsResponseModel result = apiInstance.listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet(embeddingInferenceProviderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsembeddingsApi#listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **embeddingInferenceProviderId** | [**EmbeddingInferenceProviderID**](.md)|  |

### Return type

[**ListEmbeddingInferenceProviderModelsResponseModel**](ListEmbeddingInferenceProviderModelsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


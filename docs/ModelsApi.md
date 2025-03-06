# ModelsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost**](ModelsApi.md#createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Create A Completion
[**createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost**](ModelsApi.md#createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id}/stream | Create A Streaming Completion
[**getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet**](ModelsApi.md#getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Get Model Information
[**listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet**](ModelsApi.md#listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet) | **GET** /v3/models/embeddings | List All Embedding Inference Providers
[**listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet**](ModelsApi.md#listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet) | **GET** /v3/models/llm_inference_providers | List All Llm Inference Providers
[**listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet**](ModelsApi.md#listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet) | **GET** /v3/models/embeddings/{embedding_inference_provider_id} | List Embedding Inference Provider Models
[**listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet**](ModelsApi.md#listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms | List Llm Inference Provider Models

<a name="createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost"></a>
# **createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost**
> CreateLLMCompletionResponseModel createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost(body, llmInferenceProviderId, llmModelId)

Create A Completion

Creates an LLM completion.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
CreateLLMCompletionRequestModel body = new CreateLLMCompletionRequestModel(); // CreateLLMCompletionRequestModel | 
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
LLMModelID llmModelId = new LLMModelID(); // LLMModelID | 
try {
    CreateLLMCompletionResponseModel result = apiInstance.createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost(body, llmInferenceProviderId, llmModelId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateLLMCompletionRequestModel**](CreateLLMCompletionRequestModel.md)|  |
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](.md)|  |
 **llmModelId** | [**LLMModelID**](.md)|  |

### Return type

[**CreateLLMCompletionResponseModel**](CreateLLMCompletionResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost"></a>
# **createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost**
> Object createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost(body, llmInferenceProviderId, llmModelId)

Create A Streaming Completion

Creates a streaming LLM completion.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
CreateLLMCompletionRequestModel body = new CreateLLMCompletionRequestModel(); // CreateLLMCompletionRequestModel | 
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
LLMModelID llmModelId = new LLMModelID(); // LLMModelID | 
try {
    Object result = apiInstance.createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost(body, llmInferenceProviderId, llmModelId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateLLMCompletionRequestModel**](CreateLLMCompletionRequestModel.md)|  |
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](.md)|  |
 **llmModelId** | [**LLMModelID**](.md)|  |

### Return type

**Object**

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet"></a>
# **getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet**
> GetLLMModelResponseModel getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet(llmInferenceProviderId, llmModelId)

Get Model Information

Gets information for a specified model.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
LLMModelID llmModelId = new LLMModelID(); // LLMModelID | 
try {
    GetLLMModelResponseModel result = apiInstance.getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet(llmInferenceProviderId, llmModelId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](.md)|  |
 **llmModelId** | [**LLMModelID**](.md)|  |

### Return type

[**GetLLMModelResponseModel**](GetLLMModelResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

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
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
try {
    ListEmbeddingInferenceProvidersResponseModel result = apiInstance.listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#listAllEmbeddingInferenceProvidersV3ModelsEmbeddingsGet");
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

<a name="listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet"></a>
# **listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet**
> ListLLMInferenceProvidersResponseModel listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet()

List All Llm Inference Providers

List all LLM inference providers.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
try {
    ListLLMInferenceProvidersResponseModel result = apiInstance.listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListLLMInferenceProvidersResponseModel**](ListLLMInferenceProvidersResponseModel.md)

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
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
EmbeddingInferenceProviderID embeddingInferenceProviderId = new EmbeddingInferenceProviderID(); // EmbeddingInferenceProviderID | 
try {
    ListEmbeddingInferenceProviderModelsResponseModel result = apiInstance.listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet(embeddingInferenceProviderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#listEmbeddingInferenceProviderModelsV3ModelsEmbeddingsEmbeddingInferenceProviderIdGet");
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

<a name="listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet"></a>
# **listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet**
> ListLLMInferenceProviderModelsResponseModel listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet(llmInferenceProviderId)

List Llm Inference Provider Models

Lists all LLM models in the provided llm inference provider.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ModelsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsApi apiInstance = new ModelsApi();
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
try {
    ListLLMInferenceProviderModelsResponseModel result = apiInstance.listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet(llmInferenceProviderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsApi#listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **llmInferenceProviderId** | [**LLMInferenceProviderID**](.md)|  |

### Return type

[**ListLLMInferenceProviderModelsResponseModel**](ListLLMInferenceProviderModelsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


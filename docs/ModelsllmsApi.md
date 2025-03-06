# ModelsllmsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost**](ModelsllmsApi.md#createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Create A Completion
[**createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost**](ModelsllmsApi.md#createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost) | **POST** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id}/stream | Create A Streaming Completion
[**getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet**](ModelsllmsApi.md#getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms/{llm_model_id} | Get Model Information
[**listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet**](ModelsllmsApi.md#listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet) | **GET** /v3/models/llm_inference_providers | List All Llm Inference Providers
[**listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet**](ModelsllmsApi.md#listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet) | **GET** /v3/models/llm_inference_providers/{llm_inference_provider_id}/llms | List Llm Inference Provider Models

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
//import io.swagger.client.api.ModelsllmsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsllmsApi apiInstance = new ModelsllmsApi();
CreateLLMCompletionRequestModel body = new CreateLLMCompletionRequestModel(); // CreateLLMCompletionRequestModel | 
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
LLMModelID llmModelId = new LLMModelID(); // LLMModelID | 
try {
    CreateLLMCompletionResponseModel result = apiInstance.createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost(body, llmInferenceProviderId, llmModelId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsllmsApi#createACompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdPost");
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
//import io.swagger.client.api.ModelsllmsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsllmsApi apiInstance = new ModelsllmsApi();
CreateLLMCompletionRequestModel body = new CreateLLMCompletionRequestModel(); // CreateLLMCompletionRequestModel | 
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
LLMModelID llmModelId = new LLMModelID(); // LLMModelID | 
try {
    Object result = apiInstance.createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost(body, llmInferenceProviderId, llmModelId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsllmsApi#createAStreamingCompletionV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdStreamPost");
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
//import io.swagger.client.api.ModelsllmsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsllmsApi apiInstance = new ModelsllmsApi();
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
LLMModelID llmModelId = new LLMModelID(); // LLMModelID | 
try {
    GetLLMModelResponseModel result = apiInstance.getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet(llmInferenceProviderId, llmModelId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsllmsApi#getModelInformationV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsLlmModelIdGet");
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
//import io.swagger.client.api.ModelsllmsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsllmsApi apiInstance = new ModelsllmsApi();
try {
    ListLLMInferenceProvidersResponseModel result = apiInstance.listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsllmsApi#listAllLLMInferenceProvidersV3ModelsLlmInferenceProvidersGet");
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
//import io.swagger.client.api.ModelsllmsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ModelsllmsApi apiInstance = new ModelsllmsApi();
LLMInferenceProviderID llmInferenceProviderId = new LLMInferenceProviderID(); // LLMInferenceProviderID | 
try {
    ListLLMInferenceProviderModelsResponseModel result = apiInstance.listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet(llmInferenceProviderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ModelsllmsApi#listLLMInferenceProviderModelsV3ModelsLlmInferenceProvidersLlmInferenceProviderIdLlmsGet");
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


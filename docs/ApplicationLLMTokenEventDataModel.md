# ApplicationLLMTokenEventDataModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**_id** | **Object** | The UUID of this usage event. |  [optional]
**applicationId** | **Object** | The UUID of the application associated with this usage event. | 
**inputTokens** | **Object** | The amount of input tokens used in this event. |  [optional]
**outputTokens** | **Object** | The amount of output tokens used in this event. |  [optional]
**llmModelInferenceProviderId** | [**LLMInferenceProviderID**](LLMInferenceProviderID.md) | The LLM inference provider used in this event. | 
**llmModelId** | [**LLMModelID**](LLMModelID.md) | The LLM model used in this event. | 
**createdAt** | **Object** | Event creation date. |  [optional]

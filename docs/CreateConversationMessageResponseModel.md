# CreateConversationMessageResponseModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**question** | [**ConversationMessageDataModel**](ConversationMessageDataModel.md) | The question (message) created by the user. | 
**response** | [**ConversationMessageDataModel**](ConversationMessageDataModel.md) | The response from the LLM. | 
**referenceObjectExcerpts** | **Object** |  |  [optional]
**queryPipelineId** | [**QueryPipelineID**](QueryPipelineID.md) | Used query pipeline. | 
**llmInferenceProviderId** | [**LLMInferenceProviderID**](LLMInferenceProviderID.md) | Used LLM inference provider. | 
**llmModelId** | [**LLMModelID**](LLMModelID.md) | Used LLM inference provider. | 
**usageInfo** | [**UsageInfoModel**](UsageInfoModel.md) | Request usage information. | 
**pipelineTrace** | **Object** | Pipeline trace. |  [optional]

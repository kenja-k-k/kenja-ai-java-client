# ConversationMessageDataModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**_id** | **Object** | The UUID of this conversation message. |  [optional]
**applicationId** | **Object** | The UUID of the application associated with this conversation message. | 
**conversationId** | **Object** | The UUID of the conversation associated with this conversation message. | 
**corpusId** | **Object** | The UUID of the corpus associated with this conversation message. |  [optional]
**origin** | [**ConversationMessageOrigin**](ConversationMessageOrigin.md) | The origin of this conversation message. | 
**content** | **Object** | The content of this conversation message. | 
**responseToConversationMessageId** | **Object** | The UUID of the conversation message this one is a response to. |  [optional]
**nonHallucinationScore** | **Object** | How non-hallucinatory the answer is. |  [optional]
**factualityScore** | **Object** | How factual the answer is. |  [optional]
**llmInferenceProviderId** | **Object** | The LLM inference provider associated with this message. |  [optional]
**llmModelId** | **Object** | The LLM model associated with this message. |  [optional]
**referenceObjectIds** | **Object** | Reference object UUIDs associated with this conversation message. |  [optional]
**createdAt** | **Object** | The creation date of this conversation message. |  [optional]

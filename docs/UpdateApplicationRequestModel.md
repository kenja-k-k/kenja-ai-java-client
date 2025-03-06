# UpdateApplicationRequestModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**name** | **Object** | The name of this application. | 
**organizationId** | **Object** | The UUID of the organization behind this application. | 
**apiCallsLimitPerMonth** | **Object** | The maximum amount of API calls this application can make in a month. |  [optional]
**llmTokensLimitPerMonth** | **Object** | The maximum amount of LLM tokens (combined I/O) this application can use in a month. |  [optional]
**embeddingTokensLimitPerMonth** | **Object** | The maximum amount of embedding tokens this application can use in a month. |  [optional]
**imageGenerationLimitPerMonth** | **Object** | The maximum amount of images this application can generate in a month. |  [optional]
**allowLlmQueries** | **Object** | Should this application be allowed to make queries to LLMs? |  [optional]
**allowCorpusCreation** | **Object** | Should this application be allowed to create corpuses? |  [optional]
**allowImageGeneration** | **Object** | Should this application be allowed to create images? |  [optional]
**allowExpensiveQueries** | **Object** | Should this application be allowed to make potentially expensive queries? |  [optional]
**webhookUrl** | **Object** | Webhook URL to use when notifying of queued events. |  [optional]
**isActive** | **Object** | Is this application active? |  [optional]

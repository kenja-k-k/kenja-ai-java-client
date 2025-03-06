# ApplicationDataModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**_id** | **Object** | ID of this application. |  [optional]
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
**accessKey** | **Object** | The access key for using this application. |  [optional]
**webhookUrl** | **Object** | Webhook URL to use when notifying of queued events. |  [optional]
**webhookAuthorizationKey** | **Object** | Webhook authorization key to use in order to verify the origin of webhook events. |  [optional]
**isActive** | **Object** | Is this application active? |  [optional]
**isAuthoritative** | **Object** | Is this application allowed to access management endpoints? NOTE: Usable for deployment owners only. |  [optional]
**createdAt** | **Object** | Application creation date. |  [optional]

# ReferenceObjectDataModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**_id** | **Object** | The UUID of this reference object. |  [optional]
**applicationId** | **Object** | The UUID of the application associated with this reference object. | 
**corpusId** | **Object** | The UUID of the corpus associated with this reference object. | 
**sourceId** | **Object** | The original source ID for this reference object. This field is not used internally, you can set it to any value you want. |  [optional]
**sourceName** | **Object** | The original source name for this reference object. |  [optional]
**sourceUrl** | **Object** | The original source URL for this reference object - if any. |  [optional]
**size** | **Object** | The size of this reference object (in bytes). |  [optional]
**hash** | **Object** | The hash of this reference object. This value is generated automatically, if you set it - it will be ignored. |  [optional]
**status** | [**ReferenceObjectStatus**](ReferenceObjectStatus.md) | The status of this reference object. |  [optional]
**embeddingIds** | **Object** | Embedding IDs associated with this reference object. |  [optional]
**objectType** | [**ReferenceObjectType**](ReferenceObjectType.md) | The type of this reference object. |  [optional]
**content** | **Object** | The content of the reference object (enumerated by page). |  [optional]
**summary** | **Object** | The summary of the reference object created by an LLM. |  [optional]
**createdAt** | **Object** | Creation date of this reference object. |  [optional]

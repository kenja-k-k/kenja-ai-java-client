# ReferenceObjectExcerptDataModel

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**referenceObjectId** | **Object** | The UUID of the original reference object. | 
**pageNum** | **Object** | The page number this excerpt is found at, indexed from 0. Value of -1 means pages are not supported.         This is much less useful than the actual chunk index, but users are dumb so what can you do really... |  [optional]
**offset** | **Object** | The offset at which this excerpt starts. |  [optional]
**sourceId** | **Object** | The original source ID for this reference object. This field is not used internally, you can set it to any value you want. |  [optional]
**sourceName** | **Object** | The original source name for this reference object. |  [optional]
**sourceUrl** | **Object** | The original source URL for this reference object - if any. |  [optional]
**objectType** | [**ReferenceObjectType**](ReferenceObjectType.md) | The type of this reference object. |  [optional]
**content** | **Object** | The content of the reference object excerpt. |  [optional]
**score** | **Object** | The relevance score. |  [optional]

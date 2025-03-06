# ChatbotconversationsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAConversationV3ChatbotConversationsPost**](ChatbotconversationsApi.md#createAConversationV3ChatbotConversationsPost) | **POST** /v3/chatbot/conversations | Create A Conversation
[**createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost**](ChatbotconversationsApi.md#createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost) | **POST** /v3/chatbot/conversations/{conversation_id}/messages | Create A New Message In A Conversation
[**deleteAConversationV3ChatbotConversationsConversationIdDelete**](ChatbotconversationsApi.md#deleteAConversationV3ChatbotConversationsConversationIdDelete) | **DELETE** /v3/chatbot/conversations/{conversation_id} | Delete A Conversation
[**getAConversationV3ChatbotConversationsConversationIdGet**](ChatbotconversationsApi.md#getAConversationV3ChatbotConversationsConversationIdGet) | **GET** /v3/chatbot/conversations/{conversation_id} | Get A Conversation
[**listAllConversationsV3ChatbotConversationsGet**](ChatbotconversationsApi.md#listAllConversationsV3ChatbotConversationsGet) | **GET** /v3/chatbot/conversations | List All Conversations
[**listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet**](ChatbotconversationsApi.md#listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet) | **GET** /v3/chatbot/conversations/{conversation_id}/messages | List Conversation Messages
[**updateAConversationV3ChatbotConversationsConversationIdPatch**](ChatbotconversationsApi.md#updateAConversationV3ChatbotConversationsConversationIdPatch) | **PATCH** /v3/chatbot/conversations/{conversation_id} | Update A Conversation

<a name="createAConversationV3ChatbotConversationsPost"></a>
# **createAConversationV3ChatbotConversationsPost**
> CreateConversationResponseModel createAConversationV3ChatbotConversationsPost(body)

Create A Conversation

Creates a conversation.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
CreateConversationRequestModel body = new CreateConversationRequestModel(); // CreateConversationRequestModel | 
try {
    CreateConversationResponseModel result = apiInstance.createAConversationV3ChatbotConversationsPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#createAConversationV3ChatbotConversationsPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateConversationRequestModel**](CreateConversationRequestModel.md)|  |

### Return type

[**CreateConversationResponseModel**](CreateConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost"></a>
# **createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost**
> CreateConversationMessageResponseModel createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost(body, conversationId)

Create A New Message In A Conversation

Creates a new message in a conversation along with a completion from the LLM.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
CreateConversationMessageRequestModel body = new CreateConversationMessageRequestModel(); // CreateConversationMessageRequestModel | 
Object conversationId = null; // Object | 
try {
    CreateConversationMessageResponseModel result = apiInstance.createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost(body, conversationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#createANewMessageInAConversationV3ChatbotConversationsConversationIdMessagesPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateConversationMessageRequestModel**](CreateConversationMessageRequestModel.md)|  |
 **conversationId** | [**Object**](.md)|  |

### Return type

[**CreateConversationMessageResponseModel**](CreateConversationMessageResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteAConversationV3ChatbotConversationsConversationIdDelete"></a>
# **deleteAConversationV3ChatbotConversationsConversationIdDelete**
> DeleteConversationResponseModel deleteAConversationV3ChatbotConversationsConversationIdDelete(conversationId)

Delete A Conversation

Deletes the conversation specified in &#x60;conversation_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
Object conversationId = null; // Object | 
try {
    DeleteConversationResponseModel result = apiInstance.deleteAConversationV3ChatbotConversationsConversationIdDelete(conversationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#deleteAConversationV3ChatbotConversationsConversationIdDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversationId** | [**Object**](.md)|  |

### Return type

[**DeleteConversationResponseModel**](DeleteConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAConversationV3ChatbotConversationsConversationIdGet"></a>
# **getAConversationV3ChatbotConversationsConversationIdGet**
> GetConversationResponseModel getAConversationV3ChatbotConversationsConversationIdGet(conversationId)

Get A Conversation

Returns a conversation matching the provided &#x60;conversation_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
Object conversationId = null; // Object | 
try {
    GetConversationResponseModel result = apiInstance.getAConversationV3ChatbotConversationsConversationIdGet(conversationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#getAConversationV3ChatbotConversationsConversationIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversationId** | [**Object**](.md)|  |

### Return type

[**GetConversationResponseModel**](GetConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listAllConversationsV3ChatbotConversationsGet"></a>
# **listAllConversationsV3ChatbotConversationsGet**
> ListConversationsResponseModel listAllConversationsV3ChatbotConversationsGet()

List All Conversations

Lists all conversations.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
try {
    ListConversationsResponseModel result = apiInstance.listAllConversationsV3ChatbotConversationsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#listAllConversationsV3ChatbotConversationsGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListConversationsResponseModel**](ListConversationsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet"></a>
# **listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet**
> ListConversationMessagesResponseModel listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet(conversationId)

List Conversation Messages

Lists all messages associated with a conversation specified in &#x60;conversation_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
Object conversationId = null; // Object | 
try {
    ListConversationMessagesResponseModel result = apiInstance.listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet(conversationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#listConversationMessagesV3ChatbotConversationsConversationIdMessagesGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **conversationId** | [**Object**](.md)|  |

### Return type

[**ListConversationMessagesResponseModel**](ListConversationMessagesResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateAConversationV3ChatbotConversationsConversationIdPatch"></a>
# **updateAConversationV3ChatbotConversationsConversationIdPatch**
> UpdateConversationResponseModel updateAConversationV3ChatbotConversationsConversationIdPatch(body, conversationId)

Update A Conversation

Updates the conversation specified in &#x60;conversation_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ChatbotconversationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ChatbotconversationsApi apiInstance = new ChatbotconversationsApi();
UpdateConversationRequestModel body = new UpdateConversationRequestModel(); // UpdateConversationRequestModel | 
Object conversationId = null; // Object | 
try {
    UpdateConversationResponseModel result = apiInstance.updateAConversationV3ChatbotConversationsConversationIdPatch(body, conversationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ChatbotconversationsApi#updateAConversationV3ChatbotConversationsConversationIdPatch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateConversationRequestModel**](UpdateConversationRequestModel.md)|  |
 **conversationId** | [**Object**](.md)|  |

### Return type

[**UpdateConversationResponseModel**](UpdateConversationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


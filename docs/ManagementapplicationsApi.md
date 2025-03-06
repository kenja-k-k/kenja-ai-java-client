# ManagementapplicationsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAnApplicationV3ManagementApplicationsPost**](ManagementapplicationsApi.md#createAnApplicationV3ManagementApplicationsPost) | **POST** /v3/management/applications | Create An Application
[**deleteAnApplicationV3ManagementApplicationsApplicationIdDelete**](ManagementapplicationsApi.md#deleteAnApplicationV3ManagementApplicationsApplicationIdDelete) | **DELETE** /v3/management/applications/{application_id} | Delete An Application
[**getAnApplicationV3ManagementApplicationsApplicationIdGet**](ManagementapplicationsApi.md#getAnApplicationV3ManagementApplicationsApplicationIdGet) | **GET** /v3/management/applications/{application_id} | Get An Application
[**listAllApplicationsV3ManagementApplicationsGet**](ManagementapplicationsApi.md#listAllApplicationsV3ManagementApplicationsGet) | **GET** /v3/management/applications | List All Applications
[**updateAnApplicationV3ManagementApplicationsApplicationIdPatch**](ManagementapplicationsApi.md#updateAnApplicationV3ManagementApplicationsApplicationIdPatch) | **PATCH** /v3/management/applications/{application_id} | Update An Application

<a name="createAnApplicationV3ManagementApplicationsPost"></a>
# **createAnApplicationV3ManagementApplicationsPost**
> CreateApplicationResponseModel createAnApplicationV3ManagementApplicationsPost(body)

Create An Application

Creates an application.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementapplicationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementapplicationsApi apiInstance = new ManagementapplicationsApi();
CreateApplicationRequestModel body = new CreateApplicationRequestModel(); // CreateApplicationRequestModel | 
try {
    CreateApplicationResponseModel result = apiInstance.createAnApplicationV3ManagementApplicationsPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementapplicationsApi#createAnApplicationV3ManagementApplicationsPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateApplicationRequestModel**](CreateApplicationRequestModel.md)|  |

### Return type

[**CreateApplicationResponseModel**](CreateApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json

<a name="deleteAnApplicationV3ManagementApplicationsApplicationIdDelete"></a>
# **deleteAnApplicationV3ManagementApplicationsApplicationIdDelete**
> DeleteApplicationResponseModel deleteAnApplicationV3ManagementApplicationsApplicationIdDelete(applicationId)

Delete An Application

Deletes the application specified in &#x60;application_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementapplicationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementapplicationsApi apiInstance = new ManagementapplicationsApi();
Object applicationId = null; // Object | 
try {
    DeleteApplicationResponseModel result = apiInstance.deleteAnApplicationV3ManagementApplicationsApplicationIdDelete(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementapplicationsApi#deleteAnApplicationV3ManagementApplicationsApplicationIdDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | [**Object**](.md)|  |

### Return type

[**DeleteApplicationResponseModel**](DeleteApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="getAnApplicationV3ManagementApplicationsApplicationIdGet"></a>
# **getAnApplicationV3ManagementApplicationsApplicationIdGet**
> GetApplicationResponseModel getAnApplicationV3ManagementApplicationsApplicationIdGet(applicationId)

Get An Application

Returns an application matching the provided &#x60;application_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementapplicationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementapplicationsApi apiInstance = new ManagementapplicationsApi();
Object applicationId = null; // Object | 
try {
    GetApplicationResponseModel result = apiInstance.getAnApplicationV3ManagementApplicationsApplicationIdGet(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementapplicationsApi#getAnApplicationV3ManagementApplicationsApplicationIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | [**Object**](.md)|  |

### Return type

[**GetApplicationResponseModel**](GetApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listAllApplicationsV3ManagementApplicationsGet"></a>
# **listAllApplicationsV3ManagementApplicationsGet**
> ListApplicationsResponseModel listAllApplicationsV3ManagementApplicationsGet()

List All Applications

Lists all applications.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementapplicationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementapplicationsApi apiInstance = new ManagementapplicationsApi();
try {
    ListApplicationsResponseModel result = apiInstance.listAllApplicationsV3ManagementApplicationsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementapplicationsApi#listAllApplicationsV3ManagementApplicationsGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListApplicationsResponseModel**](ListApplicationsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="updateAnApplicationV3ManagementApplicationsApplicationIdPatch"></a>
# **updateAnApplicationV3ManagementApplicationsApplicationIdPatch**
> UpdateApplicationResponseModel updateAnApplicationV3ManagementApplicationsApplicationIdPatch(body, applicationId)

Update An Application

Updates the application specified in &#x60;application_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementapplicationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementapplicationsApi apiInstance = new ManagementapplicationsApi();
UpdateApplicationRequestModel body = new UpdateApplicationRequestModel(); // UpdateApplicationRequestModel | 
Object applicationId = null; // Object | 
try {
    UpdateApplicationResponseModel result = apiInstance.updateAnApplicationV3ManagementApplicationsApplicationIdPatch(body, applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementapplicationsApi#updateAnApplicationV3ManagementApplicationsApplicationIdPatch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateApplicationRequestModel**](UpdateApplicationRequestModel.md)|  |
 **applicationId** | [**Object**](.md)|  |

### Return type

[**UpdateApplicationResponseModel**](UpdateApplicationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


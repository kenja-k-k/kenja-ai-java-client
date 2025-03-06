# ManagementApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAnApplicationV3ManagementApplicationsPost**](ManagementApi.md#createAnApplicationV3ManagementApplicationsPost) | **POST** /v3/management/applications | Create An Application
[**createAnOrganizationV3ManagementOrganizationsPost**](ManagementApi.md#createAnOrganizationV3ManagementOrganizationsPost) | **POST** /v3/management/organizations | Create An Organization
[**deleteAnApplicationV3ManagementApplicationsApplicationIdDelete**](ManagementApi.md#deleteAnApplicationV3ManagementApplicationsApplicationIdDelete) | **DELETE** /v3/management/applications/{application_id} | Delete An Application
[**deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete**](ManagementApi.md#deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete) | **DELETE** /v3/management/organizations/{organization_id} | Delete An Organization
[**getAnApplicationV3ManagementApplicationsApplicationIdGet**](ManagementApi.md#getAnApplicationV3ManagementApplicationsApplicationIdGet) | **GET** /v3/management/applications/{application_id} | Get An Application
[**getAnOrganizationV3ManagementOrganizationsOrganizationIdGet**](ManagementApi.md#getAnOrganizationV3ManagementOrganizationsOrganizationIdGet) | **GET** /v3/management/organizations/{organization_id} | Get An Organization
[**listAllApplicationsV3ManagementApplicationsGet**](ManagementApi.md#listAllApplicationsV3ManagementApplicationsGet) | **GET** /v3/management/applications | List All Applications
[**listAllOrganizationsV3ManagementOrganizationsGet**](ManagementApi.md#listAllOrganizationsV3ManagementOrganizationsGet) | **GET** /v3/management/organizations | List All Organizations
[**listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet**](ManagementApi.md#listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet) | **GET** /v3/management/organizations/{organization_id}/applications | List Organization Applications
[**updateAnApplicationV3ManagementApplicationsApplicationIdPatch**](ManagementApi.md#updateAnApplicationV3ManagementApplicationsApplicationIdPatch) | **PATCH** /v3/management/applications/{application_id} | Update An Application
[**updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch**](ManagementApi.md#updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch) | **PATCH** /v3/management/organizations/{organization_id} | Update An Organization

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
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
CreateApplicationRequestModel body = new CreateApplicationRequestModel(); // CreateApplicationRequestModel | 
try {
    CreateApplicationResponseModel result = apiInstance.createAnApplicationV3ManagementApplicationsPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#createAnApplicationV3ManagementApplicationsPost");
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

<a name="createAnOrganizationV3ManagementOrganizationsPost"></a>
# **createAnOrganizationV3ManagementOrganizationsPost**
> CreateOrganizationResponseModel createAnOrganizationV3ManagementOrganizationsPost(body)

Create An Organization

Creates an organization.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
CreateOrganizationRequestModel body = new CreateOrganizationRequestModel(); // CreateOrganizationRequestModel | 
try {
    CreateOrganizationResponseModel result = apiInstance.createAnOrganizationV3ManagementOrganizationsPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#createAnOrganizationV3ManagementOrganizationsPost");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**CreateOrganizationRequestModel**](CreateOrganizationRequestModel.md)|  |

### Return type

[**CreateOrganizationResponseModel**](CreateOrganizationResponseModel.md)

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
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
Object applicationId = null; // Object | 
try {
    DeleteApplicationResponseModel result = apiInstance.deleteAnApplicationV3ManagementApplicationsApplicationIdDelete(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#deleteAnApplicationV3ManagementApplicationsApplicationIdDelete");
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

<a name="deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete"></a>
# **deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete**
> DeleteOrganizationResponseModel deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete(organizationId)

Delete An Organization

Deletes the organization specified in &#x60;organization_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
Object organizationId = null; // Object | 
try {
    DeleteOrganizationResponseModel result = apiInstance.deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete(organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | [**Object**](.md)|  |

### Return type

[**DeleteOrganizationResponseModel**](DeleteOrganizationResponseModel.md)

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
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
Object applicationId = null; // Object | 
try {
    GetApplicationResponseModel result = apiInstance.getAnApplicationV3ManagementApplicationsApplicationIdGet(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#getAnApplicationV3ManagementApplicationsApplicationIdGet");
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

<a name="getAnOrganizationV3ManagementOrganizationsOrganizationIdGet"></a>
# **getAnOrganizationV3ManagementOrganizationsOrganizationIdGet**
> GetOrganizationResponseModel getAnOrganizationV3ManagementOrganizationsOrganizationIdGet(organizationId)

Get An Organization

Returns an organization matching the provided &#x60;organization_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
Object organizationId = null; // Object | 
try {
    GetOrganizationResponseModel result = apiInstance.getAnOrganizationV3ManagementOrganizationsOrganizationIdGet(organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#getAnOrganizationV3ManagementOrganizationsOrganizationIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | [**Object**](.md)|  |

### Return type

[**GetOrganizationResponseModel**](GetOrganizationResponseModel.md)

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
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
try {
    ListApplicationsResponseModel result = apiInstance.listAllApplicationsV3ManagementApplicationsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#listAllApplicationsV3ManagementApplicationsGet");
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

<a name="listAllOrganizationsV3ManagementOrganizationsGet"></a>
# **listAllOrganizationsV3ManagementOrganizationsGet**
> ListOrganizationsResponseModel listAllOrganizationsV3ManagementOrganizationsGet()

List All Organizations

Lists all organizations.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
try {
    ListOrganizationsResponseModel result = apiInstance.listAllOrganizationsV3ManagementOrganizationsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#listAllOrganizationsV3ManagementOrganizationsGet");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ListOrganizationsResponseModel**](ListOrganizationsResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet"></a>
# **listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet**
> ListOrganizationApplicationsResponseModel listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet(organizationId)

List Organization Applications

Lists all applications associated with an organization specified in &#x60;organization_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
Object organizationId = null; // Object | 
try {
    ListOrganizationApplicationsResponseModel result = apiInstance.listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet(organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **organizationId** | [**Object**](.md)|  |

### Return type

[**ListOrganizationApplicationsResponseModel**](ListOrganizationApplicationsResponseModel.md)

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
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
UpdateApplicationRequestModel body = new UpdateApplicationRequestModel(); // UpdateApplicationRequestModel | 
Object applicationId = null; // Object | 
try {
    UpdateApplicationResponseModel result = apiInstance.updateAnApplicationV3ManagementApplicationsApplicationIdPatch(body, applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#updateAnApplicationV3ManagementApplicationsApplicationIdPatch");
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

<a name="updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch"></a>
# **updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch**
> UpdateOrganizationResponseModel updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch(body, organizationId)

Update An Organization

Updates the organization specified in &#x60;organization_id&#x60;.

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.ManagementApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementApi apiInstance = new ManagementApi();
UpdateOrganizationRequestModel body = new UpdateOrganizationRequestModel(); // UpdateOrganizationRequestModel | 
Object organizationId = null; // Object | 
try {
    UpdateOrganizationResponseModel result = apiInstance.updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch(body, organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementApi#updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | [**UpdateOrganizationRequestModel**](UpdateOrganizationRequestModel.md)|  |
 **organizationId** | [**Object**](.md)|  |

### Return type

[**UpdateOrganizationResponseModel**](UpdateOrganizationResponseModel.md)

### Authorization

[BearerAuth](../README.md#BearerAuth)

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


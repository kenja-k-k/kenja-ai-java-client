# ManagementorganizationsApi

All URIs are relative to */*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAnOrganizationV3ManagementOrganizationsPost**](ManagementorganizationsApi.md#createAnOrganizationV3ManagementOrganizationsPost) | **POST** /v3/management/organizations | Create An Organization
[**deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete**](ManagementorganizationsApi.md#deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete) | **DELETE** /v3/management/organizations/{organization_id} | Delete An Organization
[**getAnOrganizationV3ManagementOrganizationsOrganizationIdGet**](ManagementorganizationsApi.md#getAnOrganizationV3ManagementOrganizationsOrganizationIdGet) | **GET** /v3/management/organizations/{organization_id} | Get An Organization
[**listAllOrganizationsV3ManagementOrganizationsGet**](ManagementorganizationsApi.md#listAllOrganizationsV3ManagementOrganizationsGet) | **GET** /v3/management/organizations | List All Organizations
[**listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet**](ManagementorganizationsApi.md#listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet) | **GET** /v3/management/organizations/{organization_id}/applications | List Organization Applications
[**updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch**](ManagementorganizationsApi.md#updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch) | **PATCH** /v3/management/organizations/{organization_id} | Update An Organization

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
//import io.swagger.client.api.ManagementorganizationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementorganizationsApi apiInstance = new ManagementorganizationsApi();
CreateOrganizationRequestModel body = new CreateOrganizationRequestModel(); // CreateOrganizationRequestModel | 
try {
    CreateOrganizationResponseModel result = apiInstance.createAnOrganizationV3ManagementOrganizationsPost(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementorganizationsApi#createAnOrganizationV3ManagementOrganizationsPost");
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
//import io.swagger.client.api.ManagementorganizationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementorganizationsApi apiInstance = new ManagementorganizationsApi();
Object organizationId = null; // Object | 
try {
    DeleteOrganizationResponseModel result = apiInstance.deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete(organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementorganizationsApi#deleteAnOrganizationV3ManagementOrganizationsOrganizationIdDelete");
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
//import io.swagger.client.api.ManagementorganizationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementorganizationsApi apiInstance = new ManagementorganizationsApi();
Object organizationId = null; // Object | 
try {
    GetOrganizationResponseModel result = apiInstance.getAnOrganizationV3ManagementOrganizationsOrganizationIdGet(organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementorganizationsApi#getAnOrganizationV3ManagementOrganizationsOrganizationIdGet");
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
//import io.swagger.client.api.ManagementorganizationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementorganizationsApi apiInstance = new ManagementorganizationsApi();
try {
    ListOrganizationsResponseModel result = apiInstance.listAllOrganizationsV3ManagementOrganizationsGet();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementorganizationsApi#listAllOrganizationsV3ManagementOrganizationsGet");
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
//import io.swagger.client.api.ManagementorganizationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementorganizationsApi apiInstance = new ManagementorganizationsApi();
Object organizationId = null; // Object | 
try {
    ListOrganizationApplicationsResponseModel result = apiInstance.listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet(organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementorganizationsApi#listOrganizationApplicationsV3ManagementOrganizationsOrganizationIdApplicationsGet");
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
//import io.swagger.client.api.ManagementorganizationsApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();


ManagementorganizationsApi apiInstance = new ManagementorganizationsApi();
UpdateOrganizationRequestModel body = new UpdateOrganizationRequestModel(); // UpdateOrganizationRequestModel | 
Object organizationId = null; // Object | 
try {
    UpdateOrganizationResponseModel result = apiInstance.updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch(body, organizationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ManagementorganizationsApi#updateAnOrganizationV3ManagementOrganizationsOrganizationIdPatch");
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


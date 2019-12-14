# DefaultApi

All URIs are relative to *https://virtserver.swaggerhub.com/Celestialdeath99/TRAC-Controller/1.0.0*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getStatus**](DefaultApi.md#getStatus) | **GET** /status | Get the status of all the park features
[**toggleFeature**](DefaultApi.md#toggleFeature) | **POST** /toggle | Toggle a water feature on or off

<a name="getStatus"></a>
# **getStatus**
> ArrayOfStatus getStatus()

Get the status of all the park features

Get the status of all the various waterpark features and return it as a JSON array.

### Example
```java
// Import classes:
ApiExceptionpDefaultApipi();
try {
    ArrayOfStatus result = apiInstance.getStatus();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#getStatus");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ArrayOfStatus**](ArrayOfStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a name="toggleFeature"></a>
# **toggleFeature**
> FeatureStatus toggleFeature(name)

Toggle a water feature on or off

Toggle a water feature on or off. It will be switched to whatever state it is not currently in.

### Example
```java
// Import classes:
ApiExceptApiExceptioniInstance =DefaultApi "name_example"; // String | The name of the water feature to toggle.
try {
    FeatureStatus result = apiInstance.toggleFeature(name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DefaultApi#toggleFeature");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **String**| The name of the water feature to toggle. |

### Return type

[**FeatureStatus**](FeatureStatus.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


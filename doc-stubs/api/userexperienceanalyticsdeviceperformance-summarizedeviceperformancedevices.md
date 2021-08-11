---
title: "userExperienceAnalyticsDevicePerformance: summarizeDevicePerformanceDevices"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# userExperienceAnalyticsDevicePerformance: summarizeDevicePerformanceDevices
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices
```

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|summarizeBy|userExperienceAnalyticsSummarizedBy|**TODO: Add Description**|


## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [userExperienceAnalyticsDevicePerformance](../resources/userexperienceanalyticsdeviceperformance.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "userexperienceanalyticsdeviceperformance_summarizedeviceperformancedevices"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDevicePerformance/summarizeDevicePerformanceDevices(summarizeBy='parameterValue')
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.management.services.api.userExperienceAnalyticsDevicePerformance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsDevicePerformance",
      "id": "String (identifier)",
      "deviceName": "String",
      "model": "String",
      "manufacturer": "String",
      "diskType": "String",
      "operatingSystemVersion": "String",
      "bootScore": "Integer",
      "coreBootTimeInMs": "Integer",
      "groupPolicyBootTimeInMs": "Integer",
      "healthStatus": "String",
      "loginScore": "Integer",
      "coreLoginTimeInMs": "Integer",
      "groupPolicyLoginTimeInMs": "Integer",
      "deviceCount": "Integer",
      "responsiveDesktopTimeInMs": "Integer",
      "blueScreenCount": "Integer",
      "restartCount": "Integer",
      "averageBlueScreens": "Double",
      "averageRestarts": "Double",
      "startupPerformanceScore": "Double"
    }
  ]
}
```


---
title: "Create userExperienceAnalyticsAppHealthApplicationPerformance"
description: "Create a new userExperienceAnalyticsAppHealthApplicationPerformance object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsAppHealthApplicationPerformance
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userExperienceAnalyticsAppHealthApplicationPerformance object.

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
POST /deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/userexperienceanalyticsapphealthapplicationperformance.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/userexperienceanalyticsapphealthapplicationperformance.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics app performance object.|
|appHangCount|Int32|The number of hangs for the app. Valid values -2147483648 to 2147483647|
|appHealthScore|Double|The health score of the app. Valid values -1.79769313486232E+308 to 1.79769313486232E+308|
|appHealthStatus|String|The overall health status of the app.|
|allOrgsHealthScore|Double|The median health score of the application across all organizations. Valid values -1.79769313486232E+308 to 1.79769313486232E+308|
|activeDeviceCount|Int32|The number of devices where the app has been active. Valid values -2147483648 to 2147483647|
|appName|String|The name of the application.|
|appDisplayName|String|The friendly name of the application.|
|appPublisher|String|The publisher of the application.|
|appUsageDuration|Int32|The total usage time of the application in minutes. Valid values -2147483648 to 2147483647|
|appCrashCount|Int32|The number of crashes for the app. Valid values -2147483648 to 2147483647|
|meanTimeToFailureInMinutes|Int32|The mean time to failure for the app in minutes. Valid values -2147483648 to 2147483647|



## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsAppHealthApplicationPerformance](../resources/userexperienceanalyticsapphealthapplicationperformance.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticsapphealthapplicationperformance_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthApplicationPerformance
Content-Type: application/json
Content-length: 470

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsAppHealthApplicationPerformance",
  "appHangCount": "Integer",
  "appHealthScore": "Double",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "Double",
  "activeDeviceCount": "Integer",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": "Integer",
  "appCrashCount": "Integer",
  "meanTimeToFailureInMinutes": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsAppHealthApplicationPerformance"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsAppHealthApplicationPerformance",
  "id": "be8ae5e4-e5e4-be8a-e4e5-8abee4e58abe",
  "appHangCount": "Integer",
  "appHealthScore": "Double",
  "appHealthStatus": "String",
  "allOrgsHealthScore": "Double",
  "activeDeviceCount": "Integer",
  "appName": "String",
  "appDisplayName": "String",
  "appPublisher": "String",
  "appUsageDuration": "Integer",
  "appCrashCount": "Integer",
  "meanTimeToFailureInMinutes": "Integer"
}
```


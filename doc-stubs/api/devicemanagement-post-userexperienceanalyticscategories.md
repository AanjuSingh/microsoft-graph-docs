---
title: "Create userExperienceAnalyticsCategory"
description: "Create a new userExperienceAnalyticsCategory object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userExperienceAnalyticsCategory
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userExperienceAnalyticsCategory object.

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
POST /deviceManagement/userExperienceAnalyticsCategories
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object.

The following table shows the properties that are required when you create the [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique identifier of the user experience analytics category.|
|overallScore|Int32|The overall score of the user experience analytics category.|
|totalDevices|Int32|The total device count of the user experience analytics category.|
|insights|[microsoft.management.services.api.userExperienceAnalyticsInsight](../resources/userexperienceanalyticsinsight.md) collection|The insights for the user experience analytics category.|
|state|userExperienceAnalyticsHealthState|The current health state of the user experience analytics category. Possible values are: `unknown`, `insufficientData`, `needsAttention`, `meetingGoals`.|



## Response

If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userexperienceanalyticscategory_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsCategories
Content-Type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsCategory",
  "overallScore": "Integer",
  "totalDevices": "Integer",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ],
  "state": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.userExperienceAnalyticsCategory"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.userExperienceAnalyticsCategory",
  "id": "2a751af3-1af3-2a75-f31a-752af31a752a",
  "overallScore": "Integer",
  "totalDevices": "Integer",
  "insights": [
    {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsInsight"
    }
  ],
  "state": "String"
}
```


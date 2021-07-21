---
title: "Update userExperienceAnalyticsImpactingProcess"
description: "Update the properties of a userExperienceAnalyticsImpactingProcess object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userExperienceAnalyticsImpactingProcess
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [userExperienceAnalyticsImpactingProcess](../resources/userexperienceanalyticsimpactingprocess.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsImpactingProcess](../resources/userexperienceanalyticsimpactingprocess.md) object.

The following table shows the properties that are required when you update the [userExperienceAnalyticsImpactingProcess](../resources/userexperienceanalyticsimpactingprocess.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|category|String|The category of impacting process.|
|description|String|The description of process.|
|deviceId|String|The unique identifier of the impacted device.|
|impactValue|Double|The impact value of the process. Valid values 0 to 1.79769313486232E+308|
|processName|String|The process name.|
|publisher|String|The publisher of the process.|



## Response

If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsImpactingProcess](../resources/userexperienceanalyticsimpactingprocess.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsimpactingprocess"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess/{userExperienceAnalyticsImpactingProcessId}
Content-Type: application/json
Content-length: 241

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "category": "String",
  "description": "String",
  "deviceId": "String",
  "impactValue": "Double",
  "processName": "String",
  "publisher": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
  "id": "da6b9d9f-9d9f-da6b-9f9d-6bda9f9d6bda",
  "category": "String",
  "description": "String",
  "deviceId": "String",
  "impactValue": "Double",
  "processName": "String",
  "publisher": "String"
}
```


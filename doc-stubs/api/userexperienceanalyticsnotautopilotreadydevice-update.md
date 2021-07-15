---
title: "Update userExperienceAnalyticsNotAutopilotReadyDevice"
description: "Update the properties of a userExperienceAnalyticsNotAutopilotReadyDevice object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userExperienceAnalyticsNotAutopilotReadyDevice
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/userexperienceanalyticsnotautopilotreadydevice.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/userexperienceanalyticsnotautopilotreadydevice.md) object.

The following table shows the properties that are required when you update the [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/userexperienceanalyticsnotautopilotreadydevice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|autoPilotProfileAssigned|Boolean|The intune device's autopilotProfileAssigned.|
|autoPilotRegistered|Boolean|The intune device's autopilotRegistered.|
|azureAdJoinType|String|The intune device's azure Ad joinType.|
|azureAdRegistered|Boolean|The intune device's azureAdRegistered.|
|deviceName|String|The intune device's name.|
|managedBy|String|The intune device's managed by.|
|manufacturer|String|The intune device's manufacturer.|
|model|String|The intune device's model.|
|serialNumber|String|The intune device's serial number.|



## Response

If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsNotAutopilotReadyDevice](../resources/userexperienceanalyticsnotautopilotreadydevice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsnotautopilotreadydevice"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsNotAutopilotReadyDevice/{userExperienceAnalyticsNotAutopilotReadyDeviceId}
Content-Type: application/json
Content-length: 367

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "autoPilotProfileAssigned": "Boolean",
  "autoPilotRegistered": "Boolean",
  "azureAdJoinType": "String",
  "azureAdRegistered": "Boolean",
  "deviceName": "String",
  "managedBy": "String",
  "manufacturer": "String",
  "model": "String",
  "serialNumber": "String"
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
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsNotAutopilotReadyDevice",
  "id": "9d3dda90-da90-9d3d-90da-3d9d90da3d9d",
  "autoPilotProfileAssigned": "Boolean",
  "autoPilotRegistered": "Boolean",
  "azureAdJoinType": "String",
  "azureAdRegistered": "Boolean",
  "deviceName": "String",
  "managedBy": "String",
  "manufacturer": "String",
  "model": "String",
  "serialNumber": "String"
}
```


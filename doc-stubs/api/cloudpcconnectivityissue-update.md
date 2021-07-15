---
title: "Update cloudPCConnectivityIssue"
description: "Update the properties of a cloudPCConnectivityIssue object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update cloudPCConnectivityIssue
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [cloudPCConnectivityIssue](../resources/cloudpcconnectivityissue.md) object.

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
PATCH /deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPCConnectivityIssue](../resources/cloudpcconnectivityissue.md) object.

The following table shows the properties that are required when you update the [cloudPCConnectivityIssue](../resources/cloudpcconnectivityissue.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceId|String|The Intune DeviceId of the device the connection is associated with.|
|errorCode|String|The error code of the connectivity issue.|
|errorDateTime|DateTimeOffset|The time that the connection initiated. The time is shown in ISO 8601 format and Coordinated Universal Time (UTC) time.|
|errorDescription|String|The detailed description of what went wrong.|
|recommendedAction|String|The recommended action to fix the corresponding error.|
|userId|String|The unique id of user who initialize the connection.|



## Response

If successful, this method returns a `200 OK` response code and an updated [cloudPCConnectivityIssue](../resources/cloudpcconnectivityissue.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cloudpcconnectivityissue"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues/{cloudPCConnectivityIssueId}
Content-Type: application/json
Content-length: 249

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "deviceId": "String",
  "errorCode": "String",
  "errorDateTime": "String (timestamp)",
  "errorDescription": "String",
  "recommendedAction": "String",
  "userId": "String"
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
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "e31fe5bd-e5bd-e31f-bde5-1fe3bde51fe3",
  "deviceId": "String",
  "errorCode": "String",
  "errorDateTime": "String (timestamp)",
  "errorDescription": "String",
  "recommendedAction": "String",
  "userId": "String"
}
```


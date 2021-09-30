---
title: "Create microsoftTunnelServerLogCollectionResponse"
description: "Create a new microsoftTunnelServerLogCollectionResponse object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create microsoftTunnelServerLogCollectionResponse
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new microsoftTunnelServerLogCollectionResponse object.

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
POST /deviceManagement/microsoftTunnelServerLogCollectionResponses
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [microsoftTunnelServerLogCollectionResponse](../resources/intune-microsofttunnelserverlogcollectionresponse.md) object.

The following table shows the properties that are required when you create the [microsoftTunnelServerLogCollectionResponse](../resources/intune-microsofttunnelserverlogcollectionresponse.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|The unique ID of the entity|
|status|microsoftTunnelLogCollectionStatus|The status of log collection. The possible values are: `pending`, `completed`, `failed`.|
|startDateTime|DateTimeOffset|The start time of the logs collected |
|endDateTime|DateTimeOffset|The end time of the logs collected|
|sizeInBytes|Int64|The size of the logs in bytes|
|serverId|String|ID of the server the log collection is requested upon|
|requestDateTime|DateTimeOffset|The time when the log collection was requested|
|expiryDateTime|DateTimeOffset|The time when the log collection is expired|



## Response

If successful, this method returns a `201 Created` response code and a [microsoftTunnelServerLogCollectionResponse](../resources/intune-microsofttunnelserverlogcollectionresponse.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_microsofttunnelserverlogcollectionresponse_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses
Content-Type: application/json
Content-length: 348

{
  "@odata.type": "#microsoft.management.services.api.microsoftTunnelServerLogCollectionResponse",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "sizeInBytes": "Integer",
  "serverId": "String",
  "requestDateTime": "String (timestamp)",
  "expiryDateTime": "String (timestamp)"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.management.services.api.microsoftTunnelServerLogCollectionResponse"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.management.services.api.microsoftTunnelServerLogCollectionResponse",
  "id": "69ac9583-9583-69ac-8395-ac698395ac69",
  "status": "String",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "sizeInBytes": "Integer",
  "serverId": "String",
  "requestDateTime": "String (timestamp)",
  "expiryDateTime": "String (timestamp)"
}
```


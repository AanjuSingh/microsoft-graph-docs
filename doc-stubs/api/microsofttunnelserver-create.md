---
title: "Create microsoftTunnelServer"
description: "Create a new microsoftTunnelServer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create microsoftTunnelServer
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [microsoftTunnelServer](../resources/microsofttunnelserver.md) object.

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
POST /deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [microsoftTunnelServer](../resources/microsofttunnelserver.md) object.

The following table shows the properties that are required when you create the [microsoftTunnelServer](../resources/microsofttunnelserver.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|agentImageDigest|String|The digest of the current agent image running on this server |
|displayName|String|The MicrosoftTunnelServer's display name|
|lastCheckinDateTime|DateTimeOffset|When the MicrosoftTunnelServer last checked in|
|serverImageDigest|String|The digest of the current server image running on this server |
|tunnelServerHealthStatus|microsoftTunnelServerHealthStatus|The MicrosoftTunnelServer's health status. Possible values are: `unknown`, `healthy`, `unhealthy`, `warning`, `offline`, `upgradeInProgress`, `upgradeFailed`.|



## Response

If successful, this method returns a `201 Created` response code and a [microsoftTunnelServer](../resources/microsofttunnelserver.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_microsofttunnelserver_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelSites/{microsoftTunnelSiteId}/microsoftTunnelServers
Content-Type: application/json
Content-length: 247

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "agentImageDigest": "String",
  "displayName": "String",
  "lastCheckinDateTime": "String (timestamp)",
  "serverImageDigest": "String",
  "tunnelServerHealthStatus": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.microsoftTunnelServer"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.microsoftTunnelServer",
  "id": "5cfe1c5f-1c5f-5cfe-5f1c-fe5c5f1cfe5c",
  "agentImageDigest": "String",
  "displayName": "String",
  "lastCheckinDateTime": "String (timestamp)",
  "serverImageDigest": "String",
  "tunnelServerHealthStatus": "String"
}
```


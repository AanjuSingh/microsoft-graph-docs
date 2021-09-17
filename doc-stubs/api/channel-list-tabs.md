---
title: "List tabs"
description: "Get the teamsTab resources from the tabs navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List tabs
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the teamsTab resources from the tabs navigation property.

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
GET /teams/{teamsId}/channels/{channelId}/tabs
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [teamsTab](../resources/teamstab.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_teamstab"
}
-->
``` http
GET https://graph.microsoft.com/beta/teams/{teamsId}/channels/{channelId}/tabs
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.Teams.GraphSvc.teamsTab)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Teams.GraphSvc.teamsTab",
      "id": "11c88ee3-8ee3-11c8-e38e-c811e38ec811",
      "displayName": "String",
      "teamsAppId": "String",
      "sortOrderIndex": "String",
      "messageId": "String",
      "webUrl": "String",
      "configuration": {
        "@odata.type": "microsoft.graph.teamsTabConfiguration"
      }
    }
  ]
}
```


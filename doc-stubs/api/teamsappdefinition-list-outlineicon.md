---
title: "List teamsAppIcon"
description: "Get the teamsAppIcon resources from the outlineIcon navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List teamsAppIcon
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the teamsAppIcon resources from the outlineIcon navigation property.

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
GET /chats/{chatsId}/installedApps/{teamsAppInstallationId}/teamsApp/appDefinitions/{teamsAppDefinitionId}/outlineIcon
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

If successful, this method returns a `200 OK` response code and a collection of [teamsAppIcon](../resources/teamsappicon.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_teamsappicon"
}
-->
``` http
GET https://graph.microsoft.com/beta/chats/{chatsId}/installedApps/{teamsAppInstallationId}/teamsApp/appDefinitions/{teamsAppDefinitionId}/outlineIcon
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.Teams.GraphSvc.teamsAppIcon)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Teams.GraphSvc.teamsAppIcon",
      "id": "b2790be7-0be7-b279-e70b-79b2e70b79b2",
      "webUrl": "String"
    }
  ]
}
```


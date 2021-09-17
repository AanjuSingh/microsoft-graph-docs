---
title: "Create userTeamwork"
description: "Create a new userTeamwork object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create userTeamwork
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new userTeamwork object.

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
POST /users/{usersId}/teamwork
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userTeamwork](../resources/userteamwork.md) object.

You can specify the following properties when creating a **userTeamwork**.

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Required.|



## Response

If successful, this method returns a `201 Created` response code and a [userTeamwork](../resources/userteamwork.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_userteamwork_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/teamwork
Content-Type: application/json
Content-length: 63

{
  "@odata.type": "#Microsoft.Teams.GraphSvc.userTeamwork"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.Teams.GraphSvc.userTeamwork"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.Teams.GraphSvc.userTeamwork",
  "id": "13034e6a-4e6a-1303-6a4e-03136a4e0313"
}
```


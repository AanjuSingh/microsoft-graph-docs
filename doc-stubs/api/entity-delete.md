---
title: "Delete entity"
description: "Deletes an entity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Delete entity
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Deletes an [entity](../resources/entity.md) object.

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
DELETE /me/insights/used/{usedInsightId}/resource
DELETE /me/insights/trending/{trendingId}/resource
DELETE /me/insights/shared/{sharedInsightId}/resource
DELETE /me/insights/shared/{sharedInsightId}/lastSharedMethod
DELETE /users/{usersId}/insights/used/{usedInsightId}/resource
DELETE /users/{usersId}/insights/trending/{trendingId}/resource
DELETE /users/{usersId}/insights/shared/{sharedInsightId}/resource
DELETE /users/{usersId}/insights/shared/{sharedInsightId}/lastSharedMethod
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "delete_entity"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/me/insights/used/{usedInsightId}/resource
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


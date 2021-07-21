---
title: "Update plannerDelta"
description: "Update the properties of a plannerDelta object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update plannerDelta
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [plannerDelta](../resources/plannerdelta.md) object.

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
PATCH /me/planner/all/{plannerDeltaId}
PATCH /users/{usersId}/planner/all/{plannerDeltaId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerDelta](../resources/plannerdelta.md) object.

The following table shows the properties that are required when you update the [plannerDelta](../resources/plannerdelta.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `200 OK` response code and an updated [plannerDelta](../resources/plannerdelta.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_plannerdelta"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/me/planner/all/{plannerDeltaId}
Content-Type: application/json
Content-length: 54

{
  "@odata.type": "#microsoft.graph.plannerDelta"
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
  "@odata.type": "#microsoft.graph.plannerDelta",
  "id": "57e1012a-012a-57e1-2a01-e1572a01e157"
}
```


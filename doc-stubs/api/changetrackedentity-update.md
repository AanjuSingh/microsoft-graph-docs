---
title: "Update changeTrackedEntity"
description: "Update the properties of a changeTrackedEntity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update changeTrackedEntity
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [changeTrackedEntity](../resources/changetrackedentity.md) object.

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
PATCH /changeTrackedEntity
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [changeTrackedEntity](../resources/changetrackedentity.md) object.

The following table shows the properties that are required when you update the [changeTrackedEntity](../resources/changetrackedentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|createdBy|[Microsoft.Teams.Shifts.identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|lastModifiedBy|[Microsoft.Teams.Shifts.identitySet](../resources/identityset.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [changeTrackedEntity](../resources/changetrackedentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_changetrackedentity"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/changeTrackedEntity
Content-Type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.changeTrackedEntity",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
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
  "@odata.type": "#microsoft.graph.changeTrackedEntity",
  "id": "f7062e78-2e78-f706-782e-06f7782e06f7",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


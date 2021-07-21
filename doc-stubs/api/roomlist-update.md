---
title: "Update roomList"
description: "Update the properties of a roomList object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update roomList
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [roomList](../resources/roomlist.md) object.

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
PATCH /roomList
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [roomList](../resources/roomlist.md) object.

The following table shows the properties that are required when you update the [roomList](../resources/roomlist.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|address|[physicalAddress](../resources/physicaladdress.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|displayName|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|geoCoordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|phone|String|**TODO: Add Description** Inherited from [place](../resources/place.md)|
|emailAddress|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [roomList](../resources/roomlist.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/roomList
Content-Type: application/json
Content-length: 294

{
  "@odata.type": "#microsoft.graph.roomList",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "emailAddress": "String"
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
  "@odata.type": "#microsoft.graph.roomList",
  "id": "77c8d3c2-d3c2-77c8-c2d3-c877c2d3c877",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress"
  },
  "displayName": "String",
  "geoCoordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates"
  },
  "phone": "String",
  "emailAddress": "String"
}
```


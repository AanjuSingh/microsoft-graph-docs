---
title: "Update connectorGroup"
description: "Update the properties of a connectorGroup object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update connectorGroup
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [connectorGroup](../resources/connectorgroup.md) object.

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
PATCH /applications/{applicationsId}/connectorGroup
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [connectorGroup](../resources/connectorgroup.md) object.

The following table shows the properties that are required when you update the [connectorGroup](../resources/connectorgroup.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|connectorGroupType|connectorGroupType|**TODO: Add Description**. Possible values are: `applicationProxy`.|
|isDefault|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|region|connectorGroupRegion|**TODO: Add Description**. Possible values are: `nam`, `eur`, `aus`, `asia`, `ind`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [connectorGroup](../resources/connectorgroup.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/applications/{applicationsId}/connectorGroup
Content-Type: application/json
Content-length: 162

{
  "@odata.type": "#microsoft.graph.connectorGroup",
  "connectorGroupType": "String",
  "isDefault": "Boolean",
  "name": "String",
  "region": "String"
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
  "@odata.type": "#microsoft.graph.connectorGroup",
  "id": "e3cdccd4-ccd4-e3cd-d4cc-cde3d4cccde3",
  "connectorGroupType": "String",
  "isDefault": "Boolean",
  "name": "String",
  "region": "String"
}
```


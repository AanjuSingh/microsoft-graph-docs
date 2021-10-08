---
title: "Update attributeSet"
description: "Update the properties of an attributeSet object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update attributeSet
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [attributeSet](../resources/attributeset.md) object.

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
PATCH /directory/attributeSets/{attributeSetId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [attributeSet](../resources/attributeset.md) object.

The following table shows the properties that are required when you update the [attributeSet](../resources/attributeset.md).

|Property|Type|Description|
|:---|:---|:---|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|maxAttributesPerSet|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [attributeSet](../resources/attributeset.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_attributeset"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/attributeSets/{attributeSetId}
Content-Type: application/json
Content-length: 119

{
  "@odata.type": "#microsoft.graph.attributeSet",
  "description": "String",
  "maxAttributesPerSet": "Integer"
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
  "@odata.type": "#microsoft.graph.attributeSet",
  "description": "String",
  "id": "35545fb9-5fb9-3554-b95f-5435b95f5435",
  "maxAttributesPerSet": "Integer"
}
```


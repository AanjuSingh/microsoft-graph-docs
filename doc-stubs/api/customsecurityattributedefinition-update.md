---
title: "Update customSecurityAttributeDefinition"
description: "Update the properties of a customSecurityAttributeDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update customSecurityAttributeDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) object.

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
PATCH /directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) object.

The following table shows the properties that are required when you update the [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|attributeSet|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|isCollection|Boolean|**TODO: Add Description**|
|isSearchable|Boolean|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|status|String|**TODO: Add Description**|
|type|String|**TODO: Add Description**|
|usePreDefinedValuesOnly|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [customSecurityAttributeDefinition](../resources/customsecurityattributedefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_customsecurityattributedefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/directory/customSecurityAttributeDefinitions/{customSecurityAttributeDefinitionId}
Content-Type: application/json
Content-length: 298

{
  "@odata.type": "#microsoft.graph.customSecurityAttributeDefinition",
  "attributeSet": "String",
  "description": "String",
  "isCollection": "Boolean",
  "isSearchable": "Boolean",
  "name": "String",
  "status": "String",
  "type": "String",
  "usePreDefinedValuesOnly": "Boolean"
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
  "@odata.type": "#microsoft.graph.customSecurityAttributeDefinition",
  "attributeSet": "String",
  "description": "String",
  "id": "7d3ae811-e811-7d3a-11e8-3a7d11e83a7d",
  "isCollection": "Boolean",
  "isSearchable": "Boolean",
  "name": "String",
  "status": "String",
  "type": "String",
  "usePreDefinedValuesOnly": "Boolean"
}
```


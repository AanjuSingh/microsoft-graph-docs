---
title: "Create schema"
description: "Create a new schema object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create schema
Namespace: microsoft.graph.externalConnectors

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new schema object.

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
POST /connections/{connectionsId}/schema
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [schema](../resources/externalconnectors-schema.md) object.

The following table shows the properties that are required when you create the [schema](../resources/externalconnectors-schema.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/externalconnectors-entity.md)|
|baseType|String|**TODO: Add Description**|
|properties|[microsoft.graph.externalConnectors.property](../resources/externalconnectors-property.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [schema](../resources/externalconnectors-schema.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_schema_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/connections/{connectionsId}/schema
Content-Type: application/json
Content-length: 199

{
  "@odata.type": "#microsoft.graph.externalConnectors.schema",
  "baseType": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.externalConnectors.property"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.externalConnectors.schema"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.externalConnectors.schema",
  "id": "f488d7a1-d7a1-f488-a1d7-88f4a1d788f4",
  "baseType": "String",
  "properties": [
    {
      "@odata.type": "microsoft.graph.externalConnectors.property"
    }
  ]
}
```


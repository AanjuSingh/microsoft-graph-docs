---
title: "Create onenoteEntitySchemaObjectModel"
description: "Create a new onenoteEntitySchemaObjectModel object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create onenoteEntitySchemaObjectModel
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) object.

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
POST ** Collection URI for microsoft.graph.onenoteEntitySchemaObjectModel not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) object.

The following table shows the properties that are required when you create the [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description** Inherited from [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [onenoteEntitySchemaObjectModel](../resources/onenoteentityschemaobjectmodel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_onenoteentityschemaobjectmodel_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.onenoteEntitySchemaObjectModel not found
Content-Type: application/json
Content-length: 93

{
  "@odata.type": "#microsoft.graph.onenoteEntitySchemaObjectModel",
  "self": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteEntitySchemaObjectModel"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.onenoteEntitySchemaObjectModel",
  "id": "6ea3a549-a549-6ea3-49a5-a36e49a5a36e",
  "self": "String",
  "createdDateTime": "String (timestamp)"
}
```


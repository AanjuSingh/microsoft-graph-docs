---
title: "Update onenoteEntityBaseModel"
description: "Update the properties of an onenoteEntityBaseModel object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update onenoteEntityBaseModel
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md) object.

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
PATCH /onenoteEntityBaseModel
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md) object.

The following table shows the properties that are required when you update the [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|self|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [onenoteEntityBaseModel](../resources/onenoteentitybasemodel.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_onenoteentitybasemodel"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/onenoteEntityBaseModel
Content-Type: application/json
Content-length: 85

{
  "@odata.type": "#microsoft.graph.onenoteEntityBaseModel",
  "self": "String"
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
  "@odata.type": "#microsoft.graph.onenoteEntityBaseModel",
  "id": "a0c8475d-475d-a0c8-5d47-c8a05d47c8a0",
  "self": "String"
}
```


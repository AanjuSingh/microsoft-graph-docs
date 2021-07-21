---
title: "Create inferenceClassification"
description: "Create a new inferenceClassification object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create inferenceClassification
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [inferenceClassification](../resources/inferenceclassification.md) object.

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
POST ** Collection URI for microsoft.graph.inferenceClassification not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [inferenceClassification](../resources/inferenceclassification.md) object.

The following table shows the properties that are required when you create the [inferenceClassification](../resources/inferenceclassification.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|



## Response

If successful, this method returns a `201 Created` response code and an [inferenceClassification](../resources/inferenceclassification.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_inferenceclassification_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.inferenceClassification not found
Content-Type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.inferenceClassification"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.inferenceClassification"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.inferenceClassification",
  "id": "f5738757-8757-f573-5787-73f5578773f5"
}
```


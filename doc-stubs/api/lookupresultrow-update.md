---
title: "Update lookupResultRow"
description: "Update the properties of a lookupResultRow object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update lookupResultRow
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [lookupResultRow](../resources/lookupresultrow.md) object.

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
PATCH /exactMatchLookupJob/matchingRows/{lookupResultRowId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [lookupResultRow](../resources/lookupresultrow.md) object.

The following table shows the properties that are required when you update the [lookupResultRow](../resources/lookupresultrow.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|row|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [lookupResultRow](../resources/lookupresultrow.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_lookupresultrow"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/exactMatchLookupJob/matchingRows/{lookupResultRowId}
Content-Type: application/json
Content-length: 77

{
  "@odata.type": "#microsoft.graph.lookupResultRow",
  "row": "String"
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
  "@odata.type": "#microsoft.graph.lookupResultRow",
  "id": "6b14d224-d224-6b14-24d2-146b24d2146b",
  "row": "String"
}
```


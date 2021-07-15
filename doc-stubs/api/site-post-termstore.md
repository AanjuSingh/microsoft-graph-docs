---
title: "Create store"
description: "Create a new store object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create store
Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new store object.

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
POST /sites/{sitesId}/termStore
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [store](../resources/termstore-store.md) object.

The following table shows the properties that are required when you create the [store](../resources/termstore-store.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/termstore-entity.md)|
|defaultLanguageTag|String|**TODO: Add Description**|
|languageTags|String collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [store](../resources/termstore-store.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_store_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{sitesId}/termStore
Content-Type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.termStore.store",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.store"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "44227fa2-7fa2-4422-a27f-2244a27f2244",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]
}
```


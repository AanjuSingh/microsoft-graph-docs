---
title: "Update windowsQualityUpdateCatalogItem"
description: "Update the properties of a windowsQualityUpdateCatalogItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windowsQualityUpdateCatalogItem
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [windowsQualityUpdateCatalogItem](../resources/windowsqualityupdatecatalogitem.md) object.

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
PATCH /windowsQualityUpdateCatalogItem
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsQualityUpdateCatalogItem](../resources/windowsqualityupdatecatalogitem.md) object.

The following table shows the properties that are required when you update the [windowsQualityUpdateCatalogItem](../resources/windowsqualityupdatecatalogitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The display name for the catalog item. Inherited from [windowsUpdateCatalogItem](../resources/windowsupdatecatalogitem.md)|
|endOfSupportDate|DateTimeOffset|The last supported date for a catalog item Inherited from [windowsUpdateCatalogItem](../resources/windowsupdatecatalogitem.md)|
|releaseDateTime|DateTimeOffset|The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/windowsupdatecatalogitem.md)|
|classification|windowsQualityUpdateClassification|Classification of the quality update. Possible values are: `all`, `security`, `nonSecurity`.|
|isExpeditable|Boolean|Flag indicating if update qualifies for expedite|
|kbArticleId|String|Knowledge base article id|



## Response

If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateCatalogItem](../resources/windowsqualityupdatecatalogitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windowsqualityupdatecatalogitem"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/windowsQualityUpdateCatalogItem
Content-Type: application/json
Content-length: 280

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "String",
  "endOfSupportDate": "String (timestamp)",
  "releaseDateTime": "String (timestamp)",
  "classification": "String",
  "isExpeditable": "Boolean",
  "kbArticleId": "String"
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
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "9022d2bf-d2bf-9022-bfd2-2290bfd22290",
  "displayName": "String",
  "endOfSupportDate": "String (timestamp)",
  "releaseDateTime": "String (timestamp)",
  "classification": "String",
  "isExpeditable": "Boolean",
  "kbArticleId": "String"
}
```


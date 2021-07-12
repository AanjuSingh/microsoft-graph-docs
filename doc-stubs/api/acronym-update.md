---
title: "Update acronym"
description: "Update the properties of an acronym object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update acronym
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [acronym](../resources/acronym.md) object.

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
PATCH /acronyms/{acronymsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [acronym](../resources/acronym.md) object.

The following table shows the properties that are required when you update the [acronym](../resources/acronym.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [searchAnswer](../resources/searchanswer.md)|
|displayName|String|**TODO: Add Description** Inherited from [searchAnswer](../resources/searchanswer.md)|
|description|String|**TODO: Add Description** Inherited from [searchAnswer](../resources/searchanswer.md)|
|webUrl|String|**TODO: Add Description** Inherited from [searchAnswer](../resources/searchanswer.md)|
|lastModifiedBy|[microsoft.search.admin.identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [searchAnswer](../resources/searchanswer.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [searchAnswer](../resources/searchanswer.md)|
|standsFor|String collection|**TODO: Add Description**|
|state|answerState|**TODO: Add Description**. Possible values are: `Published`, `Draft`, `Excluded`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [acronym](../resources/acronym.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_acronym"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/acronyms/{acronymsId}
Content-Type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.acronym",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "standsFor": [
    "String"
  ],
  "state": "String"
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
  "@odata.type": "#microsoft.graph.acronym",
  "id": "f85ecf0f-cf0f-f85e-0fcf-5ef80fcf5ef8",
  "displayName": "String",
  "description": "String",
  "webUrl": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "standsFor": [
    "String"
  ],
  "state": "String"
}
```


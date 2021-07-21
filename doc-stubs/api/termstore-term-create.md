---
title: "Create term"
description: "Create a new term object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create term
Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [term](../resources/termstore-term.md) object.

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
POST /sites/{sitesId}/termStore/groups/{groupId}/sets/{setId}/terms
POST /sites/{sitesId}/termStore/groups/{groupId}/sets/{setId}/children
POST /sites/{sitesId}/termStore/groups/{groupId}/sets/{setId}/children/{termId}/children
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [term](../resources/termstore-term.md) object.

The following table shows the properties that are required when you create the [term](../resources/termstore-term.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/termstore-entity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|descriptions|[microsoft.graph.termStore.localizedDescription](../resources/termstore-localizeddescription.md) collection|**TODO: Add Description**|
|labels|[microsoft.graph.termStore.localizedLabel](../resources/termstore-localizedlabel.md) collection|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|properties|[microsoft.graph.keyValue](../resources/termstore-keyvalue.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [term](../resources/termstore-term.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_term_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{sitesId}/termStore/groups/{groupId}/sets/{setId}/terms
Content-Type: application/json
Content-length: 356

{
  "@odata.type": "#microsoft.graph.termStore.term",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.termStore.term"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.termStore.term",
  "id": "d5047ee5-7ee5-d504-e57e-04d5e57e04d5",
  "createdDateTime": "String (timestamp)",
  "descriptions": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedDescription"
    }
  ],
  "labels": [
    {
      "@odata.type": "microsoft.graph.termStore.localizedLabel"
    }
  ],
  "lastModifiedDateTime": "String (timestamp)",
  "properties": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ]
}
```


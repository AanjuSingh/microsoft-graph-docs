---
title: "Update acronym"
description: "Update the properties of an acronym object."
author: "jakeost-msft"
localization_priority: Normal
ms.prod: "search"
doc_type: apiPageType
---

# Update acronym
Namespace: microsoft.graph.search

Update the properties of an [acronym](../resources/acronym.md) object.

## Permissions
One of the following permissions is required to call this api. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)| Global administrator, search administrator, search editor. |
|Delegated (personal Microsoft account)| Not supported. |
|Application| Not supported. |

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
|description|String|A brief description of the acronym that gives users more info about the acronym and what it stands for. Inherited from [searchAnswer](../resources/searchanswer.md).|
|displayName|String|The actual short form or acronym. Inherited from [searchAnswer](../resources/searchanswer.md).|
|id|String|Guid id of the acronym. Inherited from [entity](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Details of the user that created or last modified the acronym. Inherited from [searchAnswer](../resources/searchanswer.md). Read only.|
|lastModifiedDateTime|DateTimeOffset|Timestamp of when the acronym is created or edited. Inherited from [searchAnswer](../resources/searchanswer.md). Read only.|
|standsFor|String collection|What the acronym stands for.|
|state|microsoft.graph.search.answerState|State of the acronym. Possible values are: `published`, `draft`, or `excluded`.|
|webUrl|String|The url of the page or website where users can go for more information about the acronym. Inherited from [searchAnswer](../resources/searchanswer.md).|



## Response

If successful, this method returns a `204 No Content` response code.

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


{
  "description": "A deep neural network is a neural network with a certain level of complexity, a neural network with more than two layers."
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


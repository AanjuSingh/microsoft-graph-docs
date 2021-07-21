---
title: "List sitePages"
description: "Get a list of the sitePage objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List sitePages
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [sitePage](../resources/sitepage.md) objects and their properties.

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
GET /sites/{sitesId}/pages
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [sitePage](../resources/sitepage.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_sitepage"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/pages
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.sitePage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sitePage",
      "id": "3e7f78be-78be-3e7f-be78-7f3ebe787f3e",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "eTag": "String",
      "lastModifiedBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "name": "String",
      "parentReference": {
        "@odata.type": "microsoft.graph.itemReference"
      },
      "webUrl": "String",
      "contentType": {
        "@odata.type": "microsoft.graph.contentTypeInfo"
      },
      "pageLayoutType": "String",
      "publishingState": {
        "@odata.type": "microsoft.graph.publicationFacet"
      },
      "title": "String",
      "webParts": [
        {
          "@odata.type": "microsoft.graph.webPart"
        }
      ]
    }
  ]
}
```


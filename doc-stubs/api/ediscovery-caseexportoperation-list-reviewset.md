---
title: "List reviewSet"
description: "Get the reviewSet resources from the reviewSet navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List reviewSet
Namespace: microsoft.graph.ediscovery



Get the reviewSet resources from the reviewSet navigation property.

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
GET /caseExportOperation/reviewSet
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

If successful, this method returns a `200 OK` response code and a collection of [reviewSet](../resources/reviewset.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_reviewset"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/caseExportOperation/reviewSet
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.ediscovery.reviewSet)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.ediscovery.reviewSet",
      "id": "c57be7fc-e7fc-c57b-fce7-7bc5fce77bc5",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "displayName": "String",
      "createdDateTime": "String (timestamp)"
    }
  ]
}
```


---
title: "List sharePointActivityUserDetails"
description: "Get a list of the sharePointActivityUserDetail objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List sharePointActivityUserDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.sharePointActivityUserDetail not found
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

If successful, this method returns a `200 OK` response code and a collection of [sharePointActivityUserDetail](../resources/sharepointactivityuserdetail.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_sharepointactivityuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.sharePointActivityUserDetail not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.sharePointActivityUserDetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.sharePointActivityUserDetail",
      "id": "2f65cda5-cda5-2f65-a5cd-652fa5cd652f",
      "assignedProducts": [
        "String"
      ],
      "deletedDate": "Date",
      "isDeleted": "Boolean",
      "lastActivityDate": "Date",
      "reportPeriod": "String",
      "reportRefreshDate": "Date",
      "sharedExternallyFileCount": "Integer",
      "sharedInternallyFileCount": "Integer",
      "syncedFileCount": "Integer",
      "userPrincipalName": "String",
      "viewedOrEditedFileCount": "Integer",
      "visitedPageCount": "Integer"
    }
  ]
}
```


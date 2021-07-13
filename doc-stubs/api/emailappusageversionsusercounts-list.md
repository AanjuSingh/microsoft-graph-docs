---
title: "List emailAppUsageVersionsUserCounts"
description: "Get a list of the emailAppUsageVersionsUserCounts objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List emailAppUsageVersionsUserCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
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

If successful, this method returns a `200 OK` response code and a collection of [emailAppUsageVersionsUserCounts](../resources/emailappusageversionsusercounts.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_emailappusageversionsusercounts"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.emailAppUsageVersionsUserCounts not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.emailAppUsageVersionsUserCounts)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.emailAppUsageVersionsUserCounts",
      "id": "0f1eb526-b526-0f1e-26b5-1e0f26b51e0f",
      "outlook2007": "Integer",
      "outlook2010": "Integer",
      "outlook2013": "Integer",
      "outlook2016": "Integer",
      "outlook2019": "Integer",
      "outlookM365": "Integer",
      "reportPeriod": "String",
      "reportRefreshDate": "Date",
      "undetermined": "Integer"
    }
  ]
}
```


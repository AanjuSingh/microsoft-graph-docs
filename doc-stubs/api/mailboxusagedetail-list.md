---
title: "List mailboxUsageDetails"
description: "Get a list of the mailboxUsageDetail objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mailboxUsageDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [mailboxUsageDetail](../resources/mailboxusagedetail.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.mailboxUsageDetail not found
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

If successful, this method returns a `200 OK` response code and a collection of [mailboxUsageDetail](../resources/mailboxusagedetail.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_mailboxusagedetail"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.mailboxUsageDetail not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.mailboxUsageDetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mailboxUsageDetail",
      "id": "eb9ce34e-e34e-eb9c-4ee3-9ceb4ee39ceb",
      "createdDate": "Date",
      "deletedDate": "Date",
      "deletedItemCount": "Integer",
      "deletedItemSizeInBytes": "Integer",
      "displayName": "String",
      "isDeleted": "Boolean",
      "issueWarningQuotaInBytes": "Integer",
      "itemCount": "Integer",
      "lastActivityDate": "Date",
      "prohibitSendQuotaInBytes": "Integer",
      "prohibitSendReceiveQuotaInBytes": "Integer",
      "reportPeriod": "String",
      "reportRefreshDate": "Date",
      "storageUsedInBytes": "Integer",
      "userPrincipalName": "String"
    }
  ]
}
```


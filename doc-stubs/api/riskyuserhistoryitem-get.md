---
title: "Get riskyUserHistoryItem"
description: "Read the properties and relationships of a riskyUserHistoryItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get riskyUserHistoryItem
Namespace: microsoft.graph



Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

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
GET /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
GET /riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}/history/{riskyUserHistoryItemId}
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

If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/riskyUsers/{riskyUsersId}/history/{riskyUserHistoryItemId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.IdentityProtectionServices.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#Microsoft.IdentityProtectionServices.riskyUserHistoryItem",
    "id": "08c5bca4-bca4-08c5-a4bc-c508a4bcc508",
    "isDeleted": "Boolean",
    "isProcessing": "Boolean",
    "riskLastUpdatedDateTime": "String (timestamp)",
    "riskLevel": "String",
    "riskState": "String",
    "riskDetail": "String",
    "userDisplayName": "String",
    "userPrincipalName": "String",
    "userId": "String",
    "initiatedBy": "String",
    "activity": {
      "@odata.type": "microsoft.graph.riskUserActivity"
    }
  }
}
```


---
title: "List userFlowPageLayouts"
description: "Get a list of the userFlowPageLayout objects and their properties."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# List userFlowPageLayouts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [userFlowPageLayout](../resources/userflowpagelayout.md) objects and their properties.

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
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts
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

If successful, this method returns a `200 OK` response code and a collection of [userFlowPageLayout](../resources/userflowpagelayout.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_userflowpagelayout"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Microsoft.Cpim.Api.DataModels.userFlowPageLayout)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#Microsoft.Cpim.Api.DataModels.userFlowPageLayout",
      "id": "8073a745-debc-c577-dfc9-e5b451c6b227",
      "displayName": "String",
      "isCustomPageUri": "Boolean",
      "pageUri": "String",
      "version": "String"
    }
  ]
}
```


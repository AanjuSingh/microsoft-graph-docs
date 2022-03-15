---
title: "Get userFlowPageLayout"
description: "Read the properties and relationships of a userFlowPageLayout object."
author: "almars"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# Get userFlowPageLayout
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [userFlowPageLayout](../resources/userflowpagelayout.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts/{userFlowPageLayoutId}
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

If successful, this method returns a `200 OK` response code and a [userFlowPageLayout](../resources/userflowpagelayout.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_userflowpagelayout"
}
-->
``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{b2cIdentityUserFlowId}/pageLayouts/{userFlowPageLayoutId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userFlowPageLayout"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.userFlowPageLayout",
    "id": "8073a745-debc-c577-dfc9-e5b451c6b227",
    "displayName": "String",
    "isCustomPageUri": "Boolean",
    "pageUri": "String",
    "version": "String"
  }
}
```


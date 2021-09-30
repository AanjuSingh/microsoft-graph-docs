---
title: "List microsoftTunnelServerLogCollectionResponses"
description: "Get the microsoftTunnelServerLogCollectionResponse resources from the microsoftTunnelServerLogCollectionResponses navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List microsoftTunnelServerLogCollectionResponses
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the microsoftTunnelServerLogCollectionResponse resources from the microsoftTunnelServerLogCollectionResponses navigation property.

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
GET /deviceManagement/microsoftTunnelServerLogCollectionResponses
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

If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelServerLogCollectionResponse](../resources/microsofttunnelserverlogcollectionresponse.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_microsofttunnelserverlogcollectionresponse"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelServerLogCollectionResponses
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.management.services.api.microsoftTunnelServerLogCollectionResponse)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.management.services.api.microsoftTunnelServerLogCollectionResponse",
      "id": "69ac9583-9583-69ac-8395-ac698395ac69",
      "status": "String",
      "startDateTime": "String (timestamp)",
      "endDateTime": "String (timestamp)",
      "sizeInBytes": "Integer",
      "serverId": "String",
      "requestDateTime": "String (timestamp)",
      "expiryDateTime": "String (timestamp)"
    }
  ]
}
```


---
title: "List microsoftTunnelHealthThresholds"
description: "Get the microsoftTunnelHealthThreshold resources from the microsoftTunnelHealthThresholds navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List microsoftTunnelHealthThresholds
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the microsoftTunnelHealthThreshold resources from the microsoftTunnelHealthThresholds navigation property.

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
GET /deviceManagement/microsoftTunnelHealthThresholds
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

If successful, this method returns a `200 OK` response code and a collection of [microsoftTunnelHealthThreshold](../resources/microsofttunnelhealththreshold.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_microsofttunnelhealththreshold"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelHealthThresholds
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.management.services.api.microsoftTunnelHealthThreshold)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.management.services.api.microsoftTunnelHealthThreshold",
      "id": "6691d375-d375-6691-75d3-916675d39166",
      "healthyThreshold": "Integer",
      "unhealthyThreshold": "Integer",
      "defaultHealthyThreshold": "Integer",
      "defaultUnhealthyThreshold": "Integer"
    }
  ]
}
```


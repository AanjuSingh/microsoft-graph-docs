---
title: "Get printer"
description: "Read the properties and relationships of a printer object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get printer
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [printer](../resources/printer.md) object.

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
GET /print/printers/{printerId}
GET /printerCreateOperation/printer
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

If successful, this method returns a `200 OK` response code and a [printer](../resources/printer.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_printer"
}
-->
``` http
GET https://graph.microsoft.com/beta/print/printers/{printerId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.printer",
    "id": "9e7a4241-4241-9e7a-4142-7a9e41427a9e",
    "capabilities": {
      "@odata.type": "microsoft.graph.printerCapabilities"
    },
    "defaults": {
      "@odata.type": "microsoft.graph.printerDefaults"
    },
    "displayName": "String",
    "isAcceptingJobs": "Boolean",
    "location": {
      "@odata.type": "microsoft.graph.printerLocation"
    },
    "manufacturer": "String",
    "model": "String",
    "name": "String",
    "status": {
      "@odata.type": "microsoft.graph.printerStatus"
    },
    "acceptingJobs": "Boolean",
    "hasPhysicalDevice": "Boolean",
    "isShared": "Boolean",
    "lastSeenDateTime": "String (timestamp)",
    "registeredDateTime": "String (timestamp)"
  }
}
```


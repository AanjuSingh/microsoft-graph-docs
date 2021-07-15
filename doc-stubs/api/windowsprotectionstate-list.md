---
title: "List windowsProtectionStates"
description: "Get a list of the windowsProtectionState objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List windowsProtectionStates
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [windowsProtectionState](../resources/windowsprotectionstate.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.windowsProtectionState not found
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

If successful, this method returns a `200 OK` response code and a collection of [windowsProtectionState](../resources/windowsprotectionstate.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.windowsProtectionState not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsProtectionState)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsProtectionState",
      "id": "86e9e23a-e23a-86e9-3ae2-e9863ae2e986",
      "antiMalwareVersion": "String",
      "deviceState": "String",
      "engineVersion": "String",
      "fullScanOverdue": "Boolean",
      "fullScanRequired": "Boolean",
      "isVirtualMachine": "Boolean",
      "lastFullScanDateTime": "String (timestamp)",
      "lastFullScanSignatureVersion": "String",
      "lastQuickScanDateTime": "String (timestamp)",
      "lastQuickScanSignatureVersion": "String",
      "lastReportedDateTime": "String (timestamp)",
      "malwareProtectionEnabled": "Boolean",
      "networkInspectionSystemEnabled": "Boolean",
      "productStatus": "String",
      "quickScanOverdue": "Boolean",
      "realTimeProtectionEnabled": "Boolean",
      "rebootRequired": "Boolean",
      "signatureUpdateOverdue": "Boolean",
      "signatureVersion": "String",
      "tamperProtectionEnabled": "Boolean"
    }
  ]
}
```


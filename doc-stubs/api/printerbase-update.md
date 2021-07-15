---
title: "Update printerBase"
description: "Update the properties of a printerBase object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update printerBase
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [printerBase](../resources/printerbase.md) object.

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
PATCH /printerBase
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [printerBase](../resources/printerbase.md) object.

The following table shows the properties that are required when you update the [printerBase](../resources/printerbase.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|capabilities|[printerCapabilities](../resources/printercapabilities.md)|**TODO: Add Description**|
|defaults|[printerDefaults](../resources/printerdefaults.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isAcceptingJobs|Boolean|**TODO: Add Description**|
|location|[printerLocation](../resources/printerlocation.md)|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|name|String|**TODO: Add Description**|
|status|[printerStatus](../resources/printerstatus.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [printerBase](../resources/printerbase.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_printerbase"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/printerBase
Content-Type: application/json
Content-length: 498

{
  "@odata.type": "#microsoft.graph.printerBase",
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
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.printerBase",
  "id": "70ef8c22-8c22-70ef-228c-ef70228cef70",
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
  }
}
```


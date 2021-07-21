---
title: "List mobileThreatDefenseConnectors"
description: "Get a list of the mobileThreatDefenseConnector objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List mobileThreatDefenseConnectors
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) objects and their properties.

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
GET /deviceManagement/mobileThreatDefenseConnectors
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

If successful, this method returns a `200 OK` response code and a collection of [mobileThreatDefenseConnector](../resources/mobilethreatdefenseconnector.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_mobilethreatdefenseconnector"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/mobileThreatDefenseConnectors
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.mobileThreatDefenseConnector)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
      "id": "7652493d-493d-7652-3d49-52763d495276",
      "allowPartnerToCollectIOSApplicationMetadata": "Boolean",
      "androidDeviceBlockedOnMissingPartnerData": "Boolean",
      "androidEnabled": "Boolean",
      "androidMobileApplicationManagementEnabled": "Boolean",
      "iosDeviceBlockedOnMissingPartnerData": "Boolean",
      "iosEnabled": "Boolean",
      "iosMobileApplicationManagementEnabled": "Boolean",
      "lastHeartbeatDateTime": "String (timestamp)",
      "macDeviceBlockedOnMissingPartnerData": "Boolean",
      "macEnabled": "Boolean",
      "partnerState": "String",
      "partnerUnresponsivenessThresholdInDays": "Integer",
      "partnerUnsupportedOsVersionBlocked": "Boolean",
      "windowsDeviceBlockedOnMissingPartnerData": "Boolean",
      "windowsEnabled": "Boolean"
    }
  ]
}
```


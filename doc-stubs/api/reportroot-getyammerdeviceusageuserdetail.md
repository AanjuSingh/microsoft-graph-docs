---
title: "reportRoot: getYammerDeviceUsageUserDetail"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# reportRoot: getYammerDeviceUsageUserDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
GET /reports/getYammerDeviceUsageUserDetail
GET /print/reports/getYammerDeviceUsageUserDetail
```

## Function parameters
In the request URL, provide the following query parameters with values.
The following table shows the parameters that can be used with this function.

|Parameter|Type|Description|
|:---|:---|:---|
|period|String|**TODO: Add Description**|


## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail"
}
-->
``` http
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='parameterValue')
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.yammerDeviceUsageUserDetail)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.yammerDeviceUsageUserDetail",
      "id": "String (identifier)",
      "displayName": "String",
      "lastActivityDate": "Date",
      "reportPeriod": "String",
      "reportRefreshDate": "Date",
      "stateChangeDate": "Date",
      "usedAndroidPhone": "Boolean",
      "usediPad": "Boolean",
      "usediPhone": "Boolean",
      "usedOthers": "Boolean",
      "usedWeb": "Boolean",
      "usedWindowsPhone": "Boolean",
      "userPrincipalName": "String",
      "userState": "String"
    }
  ]
}
```


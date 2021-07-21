---
title: "deviceManagementReports: getAppsInstallSummaryReport"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# deviceManagementReports: getAppsInstallSummaryReport
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
POST /deviceManagement/reports/getAppsInstallSummaryReport
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|name|String|**TODO: Add Description**|
|select|String collection|**TODO: Add Description**|
|search|String|**TODO: Add Description**|
|groupBy|String collection|**TODO: Add Description**|
|orderBy|String collection|**TODO: Add Description**|
|skip|Int32|**TODO: Add Description**|
|top|Int32|**TODO: Add Description**|
|sessionId|String|**TODO: Add Description**|
|filter|String|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a Stream in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "devicemanagementreports_getappsinstallsummaryreport"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/reports/getAppsInstallSummaryReport
Content-Type: application/json
Content-length: 246

{
  "name": "String",
  "select": [
    "String"
  ],
  "search": "String",
  "groupBy": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "skip": "Integer",
  "top": "Integer",
  "sessionId": "String",
  "filter": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Edm.Stream"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": "Stream"
}
```


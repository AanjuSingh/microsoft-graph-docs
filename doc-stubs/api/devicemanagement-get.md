---
title: "Get deviceManagement"
description: "Read the properties and relationships of a deviceManagement object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get deviceManagement
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [deviceManagement](../resources/devicemanagement.md) object.

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
GET /deviceManagement
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

If successful, this method returns a `200 OK` response code and a [deviceManagement](../resources/devicemanagement.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_devicemanagement"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceManagement",
    "id": "460d18f5-18f5-460d-f518-0d46f5180d46",
    "accountMoveCompletionDateTime": "String (timestamp)",
    "adminConsent": {
      "@odata.type": "microsoft.graph.adminConsent"
    },
    "deviceComplianceReportSummarizationDateTime": "String (timestamp)",
    "deviceProtectionOverview": {
      "@odata.type": "microsoft.graph.deviceProtectionOverview"
    },
    "intuneAccountId": "Guid",
    "intuneBrand": {
      "@odata.type": "microsoft.graph.intuneBrand"
    },
    "lastReportAggregationDateTime": "String (timestamp)",
    "legacyPcManangementEnabled": "Boolean",
    "managedDeviceCleanupSettings": {
      "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
    },
    "maximumDepTokens": "Integer",
    "settings": {
      "@odata.type": "microsoft.graph.deviceManagementSettings"
    },
    "subscriptions": "String",
    "subscriptionState": "String",
    "unlicensedAdminstratorsEnabled": "Boolean",
    "userExperienceAnalyticsSettings": {
      "@odata.type": "microsoft.graph.userExperienceAnalyticsSettings"
    },
    "windowsMalwareOverview": {
      "@odata.type": "microsoft.graph.windowsMalwareOverview"
    }
  }
}
```


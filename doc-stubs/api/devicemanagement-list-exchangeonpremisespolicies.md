---
title: "List exchangeOnPremisesPolicies"
description: "Get the deviceManagementExchangeOnPremisesPolicy resources from the exchangeOnPremisesPolicies navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List exchangeOnPremisesPolicies
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the deviceManagementExchangeOnPremisesPolicy resources from the exchangeOnPremisesPolicies navigation property.

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
GET /deviceManagement/exchangeOnPremisesPolicies
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

If successful, this method returns a `200 OK` response code and a collection of [deviceManagementExchangeOnPremisesPolicy](../resources/devicemanagementexchangeonpremisespolicy.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_devicemanagementexchangeonpremisespolicy"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicies
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.deviceManagementExchangeOnPremisesPolicy)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
      "id": "8fd21135-1135-8fd2-3511-d28f3511d28f",
      "accessRules": [
        {
          "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
        }
      ],
      "defaultAccessLevel": "String",
      "knownDeviceClasses": [
        {
          "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
        }
      ],
      "notificationContent": "Binary"
    }
  ]
}
```


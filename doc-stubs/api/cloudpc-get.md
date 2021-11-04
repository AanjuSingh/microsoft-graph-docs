---
title: "Get cloudPC"
description: "Read the properties and relationships of a cloudPC object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get cloudPC
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [cloudPC](../resources/cloudpc.md) object.

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
GET /deviceManagement/virtualEndpoint/cloudPCs/{cloudPCId}
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

If successful, this method returns a `200 OK` response code and a [cloudPC](../resources/cloudpc.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_cloudpc"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/cloudPCs/{cloudPCId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPC"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.cloudPC",
    "id": "77470fcf-0fcf-7747-cf0f-4777cf0f4777",
    "displayName": "String",
    "imageDisplayName": "String",
    "aadDeviceId": "String",
    "managedDeviceId": "String",
    "managedDeviceName": "String",
    "provisioningPolicyId": "String",
    "provisioningPolicyName": "String",
    "onPremisesConnectionName": "String",
    "servicePlanId": "String",
    "servicePlanType": "String",
    "servicePlanName": "String",
    "status": "String",
    "statusDetails": {
      "@odata.type": "microsoft.graph.cloudPcStatusDetails"
    },
    "userPrincipalName": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "gracePeriodEndDateTime": "String (timestamp)",
    "lastRemoteActionResult": {
      "@odata.type": "microsoft.graph.cloudPcRemoteActionResult"
    },
    "lastLoginResult": {
      "@odata.type": "microsoft.graph.cloudPcLoginResult"
    }
  }
}
```


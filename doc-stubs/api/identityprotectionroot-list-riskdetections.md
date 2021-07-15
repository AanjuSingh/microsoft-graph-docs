---
title: "List riskDetections"
description: "Get the riskDetection resources from the riskDetections navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List riskDetections
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the riskDetection resources from the riskDetections navigation property.

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
GET /identityProtection/riskDetections
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

If successful, this method returns a `200 OK` response code and a collection of [riskDetection](../resources/riskdetection.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_riskdetection"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/riskDetections
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.riskDetection)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskDetection",
      "id": "84646c59-6c59-8464-596c-6484596c6484",
      "activity": "String",
      "activityDateTime": "String (timestamp)",
      "additionalInfo": "String",
      "correlationId": "String",
      "detectedDateTime": "String (timestamp)",
      "detectionTimingType": "String",
      "ipAddress": "String",
      "lastUpdatedDateTime": "String (timestamp)",
      "location": {
        "@odata.type": "microsoft.graph.signInLocation"
      },
      "requestId": "String",
      "riskDetail": "String",
      "riskEventType": "String",
      "riskLevel": "String",
      "riskState": "String",
      "riskType": "String",
      "source": "String",
      "tokenIssuerType": "String",
      "userDisplayName": "String",
      "userId": "String",
      "userPrincipalName": "String"
    }
  ]
}
```


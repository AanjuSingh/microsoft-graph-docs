---
title: "List provisioning"
description: "Get the provisioningObjectSummary resources from the provisioning navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List provisioning
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the provisioningObjectSummary resources from the provisioning navigation property.

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
GET /auditLogs/provisioning
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

If successful, this method returns a `200 OK` response code and a collection of [provisioningObjectSummary](../resources/provisioningobjectsummary.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_provisioningobjectsummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/auditLogs/provisioning
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.provisioningObjectSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.provisioningObjectSummary",
      "id": "63de2f2e-2f2e-63de-2e2f-de632e2fde63",
      "action": "String",
      "activityDateTime": "String (timestamp)",
      "changeId": "String",
      "cycleId": "String",
      "durationInMilliseconds": "Integer",
      "initiatedBy": {
        "@odata.type": "microsoft.graph.initiator"
      },
      "jobId": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.modifiedProperty"
        }
      ],
      "provisioningAction": "String",
      "provisioningStatusInfo": {
        "@odata.type": "microsoft.graph.provisioningStatusInfo"
      },
      "provisioningSteps": [
        {
          "@odata.type": "microsoft.graph.provisioningStep"
        }
      ],
      "servicePrincipal": {
        "@odata.type": "microsoft.graph.provisioningServicePrincipal"
      },
      "sourceIdentity": {
        "@odata.type": "microsoft.graph.provisionedIdentity"
      },
      "sourceSystem": {
        "@odata.type": "microsoft.graph.provisioningSystem"
      },
      "statusInfo": {
        "@odata.type": "microsoft.graph.statusBase"
      },
      "targetIdentity": {
        "@odata.type": "microsoft.graph.provisionedIdentity"
      },
      "targetSystem": {
        "@odata.type": "microsoft.graph.provisioningSystem"
      },
      "tenantId": "String"
    }
  ]
}
```


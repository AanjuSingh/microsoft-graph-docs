---
title: "List assignedDevices"
description: "Get the windowsAutopilotDeviceIdentity resources from the assignedDevices navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List assignedDevices
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the windowsAutopilotDeviceIdentity resources from the assignedDevices navigation property.

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
GET /deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assignedDevices
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

If successful, this method returns a `200 OK` response code and a collection of [windowsAutopilotDeviceIdentity](../resources/windowsautopilotdeviceidentity.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_windowsautopilotdeviceidentity"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeploymentProfiles/{windowsAutopilotDeploymentProfileId}/assignedDevices
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsAutopilotDeviceIdentity)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsAutopilotDeviceIdentity",
      "id": "db707176-7176-db70-7671-70db767170db",
      "addressableUserName": "String",
      "azureActiveDirectoryDeviceId": "String",
      "azureAdDeviceId": "String",
      "deploymentProfileAssignedDateTime": "String (timestamp)",
      "deploymentProfileAssignmentDetailedStatus": "String",
      "deploymentProfileAssignmentStatus": "String",
      "displayName": "String",
      "enrollmentState": "String",
      "groupTag": "String",
      "lastContactedDateTime": "String (timestamp)",
      "managedDeviceId": "String",
      "manufacturer": "String",
      "model": "String",
      "productKey": "String",
      "purchaseOrderIdentifier": "String",
      "resourceName": "String",
      "serialNumber": "String",
      "skuNumber": "String",
      "systemFamily": "String",
      "userPrincipalName": "String"
    }
  ]
}
```


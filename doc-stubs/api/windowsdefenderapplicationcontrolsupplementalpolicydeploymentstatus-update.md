---
title: "Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus"
description: "Update the properties of a windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.

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
PATCH /deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object.

The following table shows the properties that are required when you update the [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deploymentStatus|windowsDefenderApplicationControlSupplementalPolicyStatuses|The deployment state of the policy. Possible values are: `unknown`, `success`, `tokenError`, `notAuthorizedByToken`, `policyNotFound`.|
|deviceId|String|Device ID.|
|deviceName|String|Device name.|
|lastSyncDateTime|DateTimeOffset|Last sync date time.|
|osDescription|String|Windows OS Version Description.|
|osVersion|String|Windows OS Version.|
|policyVersion|String|Human readable version of the WindowsDefenderApplicationControl supplemental policy.|
|userName|String|The name of the user of this device.|
|userPrincipalName|String|User Principal Name.|



## Response

If successful, this method returns a `200 OK` response code and an updated [windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus](../resources/windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_windowsdefenderapplicationcontrolsupplementalpolicydeploymentstatus"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/wdacSupplementalPolicies/{windowsDefenderApplicationControlSupplementalPolicyId}/deviceStatuses/{windowsDefenderApplicationControlSupplementalPolicyDeploymentStatusId}
Content-Type: application/json
Content-length: 384

{
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "deploymentStatus": "String",
  "deviceId": "String",
  "deviceName": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osDescription": "String",
  "osVersion": "String",
  "policyVersion": "String",
  "userName": "String",
  "userPrincipalName": "String"
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
  "@odata.type": "#microsoft.graph.windowsDefenderApplicationControlSupplementalPolicyDeploymentStatus",
  "id": "de15db80-db80-de15-80db-15de80db15de",
  "deploymentStatus": "String",
  "deviceId": "String",
  "deviceName": "String",
  "lastSyncDateTime": "String (timestamp)",
  "osDescription": "String",
  "osVersion": "String",
  "policyVersion": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```


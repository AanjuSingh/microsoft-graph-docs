---
title: "Update comanagementEligibleDevice"
description: "Update the properties of a comanagementEligibleDevice object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update comanagementEligibleDevice
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [comanagementEligibleDevice](../resources/comanagementeligibledevice.md) object.

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
PATCH /deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [comanagementEligibleDevice](../resources/comanagementeligibledevice.md) object.

The following table shows the properties that are required when you update the [comanagementEligibleDevice](../resources/comanagementeligibledevice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|clientRegistrationStatus|deviceRegistrationState|ClientRegistrationStatus. Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`.|
|deviceName|String|DeviceName|
|deviceType|deviceType|DeviceType. Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `chromeOS`, `linux`, `blackberry`, `palm`, `unknown`, `cloudPC`.|
|entitySource|Int32|EntitySource|
|managementAgents|managementAgentType|ManagementAgents. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`, `microsoft365ManagedMdm`, `windowsManagementCloudApi`, `intuneAosp`.|
|managementState|managementState|ManagementState. Possible values are: `managed`, `retirePending`, `retireFailed`, `wipePending`, `wipeFailed`, `unhealthy`, `deletePending`, `retireIssued`, `wipeIssued`, `wipeCanceled`, `retireCanceled`, `discovered`.|
|manufacturer|String|Manufacturer|
|mdmStatus|String|MDMStatus|
|model|String|Model|
|osDescription|String|OSDescription|
|osVersion|String|OSVersion|
|ownerType|ownerType|OwnerType. Possible values are: `unknown`, `company`, `personal`.|
|referenceId|String|ReferenceId|
|serialNumber|String|SerialNumber|
|status|comanagementEligibleType|ComanagementEligibleStatus. Possible values are: `comanaged`, `eligible`, `eligibleButNotAzureAdJoined`, `needsOsUpdate`, `ineligible`.|
|upn|String|UPN|
|userEmail|String|UserEmail|
|userId|String|UserId|
|userName|String|UserName|



## Response

If successful, this method returns a `200 OK` response code and an updated [comanagementEligibleDevice](../resources/comanagementeligibledevice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_comanagementeligibledevice"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/comanagementEligibleDevices/{comanagementEligibleDeviceId}
Content-Type: application/json
Content-length: 591

{
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "clientRegistrationStatus": "String",
  "deviceName": "String",
  "deviceType": "String",
  "entitySource": "Integer",
  "managementAgents": "String",
  "managementState": "String",
  "manufacturer": "String",
  "mdmStatus": "String",
  "model": "String",
  "osDescription": "String",
  "osVersion": "String",
  "ownerType": "String",
  "referenceId": "String",
  "serialNumber": "String",
  "status": "String",
  "upn": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String"
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
  "@odata.type": "#microsoft.graph.comanagementEligibleDevice",
  "id": "819c4497-4497-819c-9744-9c8197449c81",
  "clientRegistrationStatus": "String",
  "deviceName": "String",
  "deviceType": "String",
  "entitySource": "Integer",
  "managementAgents": "String",
  "managementState": "String",
  "manufacturer": "String",
  "mdmStatus": "String",
  "model": "String",
  "osDescription": "String",
  "osVersion": "String",
  "ownerType": "String",
  "referenceId": "String",
  "serialNumber": "String",
  "status": "String",
  "upn": "String",
  "userEmail": "String",
  "userId": "String",
  "userName": "String"
}
```


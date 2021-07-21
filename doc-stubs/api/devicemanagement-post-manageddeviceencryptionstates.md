---
title: "Create managedDeviceEncryptionState"
description: "Create a new managedDeviceEncryptionState object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create managedDeviceEncryptionState
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new managedDeviceEncryptionState object.

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
POST /deviceManagement/managedDeviceEncryptionStates
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object.

The following table shows the properties that are required when you create the [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|advancedBitLockerStates|advancedBitLockerState|Advanced BitLocker State. Possible values are: `success`, `noUserConsent`, `osVolumeUnprotected`, `osVolumeTpmRequired`, `osVolumeTpmOnlyRequired`, `osVolumeTpmPinRequired`, `osVolumeTpmStartupKeyRequired`, `osVolumeTpmPinStartupKeyRequired`, `osVolumeEncryptionMethodMismatch`, `recoveryKeyBackupFailed`, `fixedDriveNotEncrypted`, `fixedDriveEncryptionMethodMismatch`, `loggedOnUserNonAdmin`, `windowsRecoveryEnvironmentNotConfigured`, `tpmNotAvailable`, `tpmNotReady`, `networkError`.|
|deviceName|String|Device name|
|deviceType|deviceTypes|Platform of the device. Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.|
|encryptionPolicySettingState|complianceStatus|Encryption policy setting state. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|encryptionReadinessState|encryptionReadinessState|Encryption readiness state. Possible values are: `notReady`, `ready`.|
|encryptionState|encryptionState|Device encryption state. Possible values are: `notEncrypted`, `encrypted`.|
|fileVaultStates|fileVaultState|FileVault State. Possible values are: `success`, `driveEncryptedByUser`, `userDeferredEncryption`, `escrowNotEnabled`.|
|osVersion|String|Operating system version of the device|
|policyDetails|[encryptionReportPolicyDetails](../resources/encryptionreportpolicydetails.md) collection|Policy Details|
|tpmSpecificationVersion|String|Device TPM Version|
|userPrincipalName|String|User name|



## Response

If successful, this method returns a `201 Created` response code and a [managedDeviceEncryptionState](../resources/manageddeviceencryptionstate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_manageddeviceencryptionstate_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
Content-Type: application/json
Content-length: 526

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "advancedBitLockerStates": "String",
  "deviceName": "String",
  "deviceType": "String",
  "encryptionPolicySettingState": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "fileVaultStates": "String",
  "osVersion": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
    }
  ],
  "tpmSpecificationVersion": "String",
  "userPrincipalName": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedDeviceEncryptionState"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
  "id": "c15094c0-94c0-c150-c094-50c1c09450c1",
  "advancedBitLockerStates": "String",
  "deviceName": "String",
  "deviceType": "String",
  "encryptionPolicySettingState": "String",
  "encryptionReadinessState": "String",
  "encryptionState": "String",
  "fileVaultStates": "String",
  "osVersion": "String",
  "policyDetails": [
    {
      "@odata.type": "microsoft.graph.encryptionReportPolicyDetails"
    }
  ],
  "tpmSpecificationVersion": "String",
  "userPrincipalName": "String"
}
```


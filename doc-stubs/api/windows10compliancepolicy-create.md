---
title: "Create windows10CompliancePolicy"
description: "Create a new windows10CompliancePolicy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windows10CompliancePolicy
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [windows10CompliancePolicy](../resources/windows10compliancepolicy.md) object.

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
POST ** Collection URI for microsoft.graph.windows10CompliancePolicy not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windows10CompliancePolicy](../resources/windows10compliancepolicy.md) object.

The following table shows the properties that are required when you create the [windows10CompliancePolicy](../resources/windows10compliancepolicy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceCompliancePolicy](../resources/devicecompliancepolicy.md)|
|activeFirewallRequired|Boolean|Require active firewall on Windows devices.|
|antiSpywareRequired|Boolean|Require any AntiSpyware solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).|
|antivirusRequired|Boolean|Require any Antivirus solution registered with Windows Decurity Center to be on and monitoring (e.g. Symantec, Windows Defender).|
|bitLockerEnabled|Boolean|Require devices to be reported healthy by Windows Device Health Attestation - bit locker is enabled|
|codeIntegrityEnabled|Boolean|Require devices to be reported as healthy by Windows Device Health Attestation.|
|configurationManagerComplianceRequired|Boolean|Require to consider SCCM Compliance state into consideration for Intune Compliance State.|
|defenderEnabled|Boolean|Require Windows Defender Antimalware on Windows devices.|
|defenderVersion|String|Require Windows Defender Antimalware minimum version on Windows devices.|
|deviceCompliancePolicyScript|[deviceCompliancePolicyScript](../resources/devicecompliancepolicyscript.md)|**TODO: Add Description**|
|deviceThreatProtectionEnabled|Boolean|Require that devices have enabled device threat protection.|
|deviceThreatProtectionRequiredSecurityLevel|deviceThreatProtectionLevel|Require Device Threat Protection minimum risk level to report noncompliance. Possible values are: `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`.|
|earlyLaunchAntiMalwareDriverEnabled|Boolean|Require devices to be reported as healthy by Windows Device Health Attestation - early launch antimalware driver is enabled.|
|mobileOsMaximumVersion|String|Maximum Windows Phone version.|
|mobileOsMinimumVersion|String|Minimum Windows Phone version.|
|osMaximumVersion|String|Maximum Windows 10 version.|
|osMinimumVersion|String|Minimum Windows 10 version.|
|passwordBlockSimple|Boolean|Indicates whether or not to block simple password.|
|passwordExpirationDays|Int32|The password expiration in days.|
|passwordMinimumCharacterSetCount|Int32|The number of character sets required in the password.|
|passwordMinimumLength|Int32|The minimum password length.|
|passwordMinutesOfInactivityBeforeLock|Int32|Minutes of inactivity before a password is required.|
|passwordPreviousPasswordBlockCount|Int32|The number of previous passwords to prevent re-use of.|
|passwordRequired|Boolean|Require a password to unlock Windows device.|
|passwordRequiredToUnlockFromIdle|Boolean|Require a password to unlock an idle device.|
|passwordRequiredType|requiredPasswordType|The required password type. Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.|
|requireHealthyDeviceReport|Boolean|Require devices to be reported as healthy by Windows Device Health Attestation.|
|rtpEnabled|Boolean|Require Windows Defender Antimalware Real-Time Protection on Windows devices.|
|secureBootEnabled|Boolean|Require devices to be reported as healthy by Windows Device Health Attestation - secure boot is enabled.|
|signatureOutOfDate|Boolean|Require Windows Defender Antimalware Signature to be up to date on Windows devices.|
|storageRequireEncryption|Boolean|Require encryption on windows devices.|
|tpmRequired|Boolean|Require Trusted Platform Module(TPM) to be present.|
|validOperatingSystemBuildRanges|[operatingSystemVersionRange](../resources/operatingsystemversionrange.md) collection|The valid operating system build ranges on Windows devices. This collection can contain a maximum of 10000 elements.|



## Response

If successful, this method returns a `201 Created` response code and a [windows10CompliancePolicy](../resources/windows10compliancepolicy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windows10compliancepolicy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.windows10CompliancePolicy not found
Content-Type: application/json
Content-length: 1647

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "description": "String",
  "displayName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer",
  "activeFirewallRequired": "Boolean",
  "antiSpywareRequired": "Boolean",
  "antivirusRequired": "Boolean",
  "bitLockerEnabled": "Boolean",
  "codeIntegrityEnabled": "Boolean",
  "configurationManagerComplianceRequired": "Boolean",
  "defenderEnabled": "Boolean",
  "defenderVersion": "String",
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript"
  },
  "deviceThreatProtectionEnabled": "Boolean",
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "earlyLaunchAntiMalwareDriverEnabled": "Boolean",
  "mobileOsMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "osMaximumVersion": "String",
  "osMinimumVersion": "String",
  "passwordBlockSimple": "Boolean",
  "passwordExpirationDays": "Integer",
  "passwordMinimumCharacterSetCount": "Integer",
  "passwordMinimumLength": "Integer",
  "passwordMinutesOfInactivityBeforeLock": "Integer",
  "passwordPreviousPasswordBlockCount": "Integer",
  "passwordRequired": "Boolean",
  "passwordRequiredToUnlockFromIdle": "Boolean",
  "passwordRequiredType": "String",
  "requireHealthyDeviceReport": "Boolean",
  "rtpEnabled": "Boolean",
  "secureBootEnabled": "Boolean",
  "signatureOutOfDate": "Boolean",
  "storageRequireEncryption": "Boolean",
  "tpmRequired": "Boolean",
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windows10CompliancePolicy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windows10CompliancePolicy",
  "id": "4eeeddd0-ddd0-4eee-d0dd-ee4ed0ddee4e",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer",
  "activeFirewallRequired": "Boolean",
  "antiSpywareRequired": "Boolean",
  "antivirusRequired": "Boolean",
  "bitLockerEnabled": "Boolean",
  "codeIntegrityEnabled": "Boolean",
  "configurationManagerComplianceRequired": "Boolean",
  "defenderEnabled": "Boolean",
  "defenderVersion": "String",
  "deviceCompliancePolicyScript": {
    "@odata.type": "microsoft.graph.deviceCompliancePolicyScript"
  },
  "deviceThreatProtectionEnabled": "Boolean",
  "deviceThreatProtectionRequiredSecurityLevel": "String",
  "earlyLaunchAntiMalwareDriverEnabled": "Boolean",
  "mobileOsMaximumVersion": "String",
  "mobileOsMinimumVersion": "String",
  "osMaximumVersion": "String",
  "osMinimumVersion": "String",
  "passwordBlockSimple": "Boolean",
  "passwordExpirationDays": "Integer",
  "passwordMinimumCharacterSetCount": "Integer",
  "passwordMinimumLength": "Integer",
  "passwordMinutesOfInactivityBeforeLock": "Integer",
  "passwordPreviousPasswordBlockCount": "Integer",
  "passwordRequired": "Boolean",
  "passwordRequiredToUnlockFromIdle": "Boolean",
  "passwordRequiredType": "String",
  "requireHealthyDeviceReport": "Boolean",
  "rtpEnabled": "Boolean",
  "secureBootEnabled": "Boolean",
  "signatureOutOfDate": "Boolean",
  "storageRequireEncryption": "Boolean",
  "tpmRequired": "Boolean",
  "validOperatingSystemBuildRanges": [
    {
      "@odata.type": "microsoft.graph.operatingSystemVersionRange"
    }
  ]
}
```


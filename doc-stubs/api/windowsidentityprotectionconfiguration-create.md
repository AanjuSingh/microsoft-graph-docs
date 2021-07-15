---
title: "Create windowsIdentityProtectionConfiguration"
description: "Create a new windowsIdentityProtectionConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create windowsIdentityProtectionConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [windowsIdentityProtectionConfiguration](../resources/windowsidentityprotectionconfiguration.md) object.

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
POST ** Collection URI for microsoft.graph.windowsIdentityProtectionConfiguration not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [windowsIdentityProtectionConfiguration](../resources/windowsidentityprotectionconfiguration.md) object.

The following table shows the properties that are required when you create the [windowsIdentityProtectionConfiguration](../resources/windowsidentityprotectionconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|DateTime the object was created. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|description|String|Admin provided description of the Device Configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleDeviceMode|[deviceManagementApplicabilityRuleDeviceMode](../resources/devicemanagementapplicabilityruledevicemode.md)|The device mode applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsEdition|[deviceManagementApplicabilityRuleOsEdition](../resources/devicemanagementapplicabilityruleosedition.md)|The OS edition applicability for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|deviceManagementApplicabilityRuleOsVersion|[deviceManagementApplicabilityRuleOsVersion](../resources/devicemanagementapplicabilityruleosversion.md)|The OS version applicability rule for this Policy. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|displayName|String|Admin provided name of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|supportsScopeTags|Boolean|Indicates whether or not the underlying Device Configuration supports the assignment of scope tags. Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users. This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal. This property is read-only. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|version|Int32|Version of the device configuration. Inherited from [deviceConfiguration](../resources/deviceconfiguration.md)|
|enhancedAntiSpoofingForFacialFeaturesEnabled|Boolean|Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.|
|pinExpirationInDays|Int32|Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it. Valid values are 0 to 730 inclusive. Valid values 0 to 730|
|pinLowercaseCharactersUsage|configurationUsage|This value configures the use of lowercase characters in the Windows Hello for Business PIN. Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinMaximumLength|Int32|Integer value that sets the maximum number of characters allowed for the work PIN. Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN. Valid values 4 to 127|
|pinMinimumLength|Int32|Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN. Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN. Valid values 4 to 127|
|pinPreviousBlockCount|Int32|Controls the ability to prevent users from using past PINs. This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count. If set to 0, previous PINs are not stored. PIN history is not preserved through a PIN reset. Valid values 0 to 50|
|pinRecoveryEnabled|Boolean|Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.|
|pinSpecialCharactersUsage|configurationUsage|Controls the ability to use special characters in the Windows Hello for Business PIN. Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.|
|pinUppercaseCharactersUsage|configurationUsage|This value configures the use of uppercase characters in the Windows Hello for Business PIN. Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.|
|securityDeviceRequired|Boolean|Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business. A TPM provides an additional security benefit in that data stored on it cannot be used on other devices. If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.|
|unlockWithBiometricsEnabled|Boolean|Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN. If set to False, biometric gestures are not allowed. Users must still configure a PIN as a backup in case of failures.|
|useCertificatesForOnPremisesAuthEnabled|Boolean|Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.|
|useSecurityKeyForSignin|Boolean|Boolean value used to enable the Windows Hello security key as a logon credential.|
|windowsHelloForBusinessBlocked|Boolean|Boolean value that blocks Windows Hello for Business as a method for signing into Windows.|



## Response

If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/windowsidentityprotectionconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_windowsidentityprotectionconfiguration_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.windowsIdentityProtectionConfiguration not found
Content-Type: application/json
Content-length: 1259

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "description": "String",
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "displayName": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": "Boolean",
  "version": "Integer",
  "enhancedAntiSpoofingForFacialFeaturesEnabled": "Boolean",
  "pinExpirationInDays": "Integer",
  "pinLowercaseCharactersUsage": "String",
  "pinMaximumLength": "Integer",
  "pinMinimumLength": "Integer",
  "pinPreviousBlockCount": "Integer",
  "pinRecoveryEnabled": "Boolean",
  "pinSpecialCharactersUsage": "String",
  "pinUppercaseCharactersUsage": "String",
  "securityDeviceRequired": "Boolean",
  "unlockWithBiometricsEnabled": "Boolean",
  "useCertificatesForOnPremisesAuthEnabled": "Boolean",
  "useSecurityKeyForSignin": "Boolean",
  "windowsHelloForBusinessBlocked": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsIdentityProtectionConfiguration"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "89242d26-2d26-8924-262d-2489262d2489",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
  },
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
  },
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": "Boolean",
  "version": "Integer",
  "enhancedAntiSpoofingForFacialFeaturesEnabled": "Boolean",
  "pinExpirationInDays": "Integer",
  "pinLowercaseCharactersUsage": "String",
  "pinMaximumLength": "Integer",
  "pinMinimumLength": "Integer",
  "pinPreviousBlockCount": "Integer",
  "pinRecoveryEnabled": "Boolean",
  "pinSpecialCharactersUsage": "String",
  "pinUppercaseCharactersUsage": "String",
  "securityDeviceRequired": "Boolean",
  "unlockWithBiometricsEnabled": "Boolean",
  "useCertificatesForOnPremisesAuthEnabled": "Boolean",
  "useSecurityKeyForSignin": "Boolean",
  "windowsHelloForBusinessBlocked": "Boolean"
}
```


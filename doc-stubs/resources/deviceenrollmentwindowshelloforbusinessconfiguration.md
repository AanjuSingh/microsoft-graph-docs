---
title: "deviceEnrollmentWindowsHelloForBusinessConfiguration resource type"
description: "Windows Hello for Business settings lets users access their devices using a gesture, such as biometric authentication, or a PIN. Configure settings for enrolled Windows 10, Windows 10 Mobile and later."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceEnrollmentWindowsHelloForBusinessConfiguration resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows Hello for Business settings lets users access their devices using a gesture, such as biometric authentication, or a PIN. Configure settings for enrolled Windows 10, Windows 10 Mobile and later.


Inherits from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceEnrollmentWindowsHelloForBusinessConfigurations](../api/deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) collection|Get a list of the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) objects and their properties.|
|[Create deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md)|Create a new [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[Get deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md)|Read the properties and relationships of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[Update deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md)|Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[Delete deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|None|Deletes a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/deviceenrollmentwindowshelloforbusinessconfiguration.md) object.|
|[assign](../api/deviceenrollmentwindowshelloforbusinessconfiguration-assign.md)|None|**TODO: Add Description**|
|[setPriority](../api/deviceenrollmentwindowshelloforbusinessconfiguration-setpriority.md)|None|**TODO: Add Description**|
|[List assignments](../api/deviceenrollmentwindowshelloforbusinessconfiguration-list-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|Get the enrollmentConfigurationAssignment resources from the assignments navigation property.|
|[Create enrollmentConfigurationAssignment](../api/deviceenrollmentwindowshelloforbusinessconfiguration-post-assignments.md)|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md)|Create a new enrollmentConfigurationAssignment object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|
|description|String|The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|
|displayName|String|The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|
|enhancedBiometricsState|enablement|Controls the ability to use the anti-spoofing features for facial recognition on devices which support it. If set to disabled, anti-spoofing features are not allowed. If set to Not Configured, the user can choose whether they want to use anti-spoofing. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|
|pinExpirationInDays|Int32|Controls the period of time (in days) that a PIN can be used before the system requires the user to change it. This must be set between 0 and 730, inclusive. If set to 0, the user's PIN will never expire|
|pinLowercaseCharactersUsage|windowsHelloForBusinessPinUsage|Controls the ability to use lowercase letters in the Windows Hello for Business PIN. Allowed permits the use of lowercase letter(s), whereas Required ensures they are present. If set to Not Allowed, lowercase letters will not be permitted. Possible values are: `allowed`, `required`, `disallowed`.|
|pinMaximumLength|Int32|Controls the maximum number of characters allowed for the Windows Hello for Business PIN. This value must be between 4 and 127, inclusive. This value must be greater than or equal to the value set for the minimum PIN.|
|pinMinimumLength|Int32|Controls the minimum number of characters required for the Windows Hello for Business PIN. This value must be between 4 and 127, inclusive, and less than or equal to the value set for the maximum PIN.|
|pinPreviousBlockCount|Int32|Controls the ability to prevent users from using past PINs. This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count. If set to 0, previous PINs are not stored. PIN history is not preserved through a PIN reset.|
|pinSpecialCharactersUsage|windowsHelloForBusinessPinUsage|Controls the ability to use special characters in the Windows Hello for Business PIN. Allowed permits the use of special character(s), whereas Required ensures they are present. If set to Not Allowed, special character(s) will not be permitted. Possible values are: `allowed`, `required`, `disallowed`.|
|pinUppercaseCharactersUsage|windowsHelloForBusinessPinUsage|Controls the ability to use uppercase letters in the Windows Hello for Business PIN. Allowed permits the use of uppercase letter(s), whereas Required ensures they are present. If set to Not Allowed, uppercase letters will not be permitted. Possible values are: `allowed`, `required`, `disallowed`.|
|priority|Int32|Priority is used when a user exists in multiple groups that are assigned enrollment configuration. Users are subject only to the configuration with the lowest priority value. Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|
|remotePassportEnabled|Boolean|Controls the use of Remote Windows Hello for Business. Remote Windows Hello for Business provides the ability for a portable, registered device to be usable as a companion for desktop authentication. The desktop must be Azure AD joined and the companion device must have a Windows Hello for Business PIN.|
|roleScopeTagIds|String collection|Optional role scope tags for the enrollment restrictions. Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|
|securityDeviceRequired|Boolean|Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business. A TPM provides an additional security benefit in that data stored on it cannot be used on other devices. If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.|
|securityKeyForSignIn|enablement|Security key for Sign In provides the capacity for remotely turning ON/OFF Windows Hello Sercurity Keyl Not configured will honor configurations done on the clinet. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|state|enablement|Controls whether to allow the device to be configured for Windows Hello for Business. If set to disabled, the user cannot provision Windows Hello for Business except on Azure Active Directory joined mobile phones if otherwise required. If set to Not Configured, Intune will not override client defaults. Possible values are: `notConfigured`, `enabled`, `disabled`.|
|unlockWithBiometricsEnabled|Boolean|Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN. If set to False, biometric gestures are not allowed. Users must still configure a PIN as a backup in case of failures.|
|version|Int32|The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[enrollmentConfigurationAssignment](../resources/enrollmentconfigurationassignment.md) collection|The list of group assignments for the device configuration profile Inherited from [deviceEnrollmentConfiguration](../resources/deviceenrollmentconfiguration.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "baseType": "microsoft.graph.deviceEnrollmentConfiguration",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "priority": "Integer",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "Integer",
  "enhancedBiometricsState": "String",
  "pinExpirationInDays": "Integer",
  "pinLowercaseCharactersUsage": "String",
  "pinMaximumLength": "Integer",
  "pinMinimumLength": "Integer",
  "pinPreviousBlockCount": "Integer",
  "pinSpecialCharactersUsage": "String",
  "pinUppercaseCharactersUsage": "String",
  "remotePassportEnabled": "Boolean",
  "securityDeviceRequired": "Boolean",
  "securityKeyForSignIn": "String",
  "state": "String",
  "unlockWithBiometricsEnabled": "Boolean"
}
```


---
title: "Get defaultManagedAppProtection"
description: "Read the properties and relationships of a defaultManagedAppProtection object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get defaultManagedAppProtection
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) object.

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
GET /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
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

If successful, this method returns a `200 OK` response code and a [defaultManagedAppProtection](../resources/defaultmanagedappprotection.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_defaultmanagedappprotection"
}
-->
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.defaultManagedAppProtection"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
    "id": "a6bea386-a386-a6be-86a3-bea686a3bea6",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "displayName": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "roleScopeTagIds": [
      "String"
    ],
    "version": "String",
    "allowedDataIngestionLocations": [
      "String"
    ],
    "allowedDataStorageLocations": [
      "String"
    ],
    "allowedInboundDataTransferSources": "String",
    "allowedOutboundClipboardSharingExceptionLength": "Integer",
    "allowedOutboundClipboardSharingLevel": "String",
    "allowedOutboundDataTransferDestinations": "String",
    "appActionIfDeviceComplianceRequired": "String",
    "appActionIfMaximumPinRetriesExceeded": "String",
    "appActionIfUnableToAuthenticateUser": "String",
    "blockDataIngestionIntoOrganizationDocuments": "Boolean",
    "contactSyncBlocked": "Boolean",
    "dataBackupBlocked": "Boolean",
    "deviceComplianceRequired": "Boolean",
    "dialerRestrictionLevel": "String",
    "disableAppPinIfDevicePinIsSet": "Boolean",
    "fingerprintBlocked": "Boolean",
    "managedBrowser": "String",
    "managedBrowserToOpenLinksRequired": "Boolean",
    "maximumAllowedDeviceThreatLevel": "String",
    "maximumPinRetries": "Integer",
    "maximumRequiredOsVersion": "String",
    "maximumWarningOsVersion": "String",
    "maximumWipeOsVersion": "String",
    "minimumPinLength": "Integer",
    "minimumRequiredAppVersion": "String",
    "minimumRequiredOsVersion": "String",
    "minimumWarningAppVersion": "String",
    "minimumWarningOsVersion": "String",
    "minimumWipeAppVersion": "String",
    "minimumWipeOsVersion": "String",
    "mobileThreatDefenseRemediationAction": "String",
    "notificationRestriction": "String",
    "organizationalCredentialsRequired": "Boolean",
    "periodBeforePinReset": "String (duration)",
    "periodOfflineBeforeAccessCheck": "String (duration)",
    "periodOfflineBeforeWipeIsEnforced": "String (duration)",
    "periodOnlineBeforeAccessCheck": "String (duration)",
    "pinCharacterSet": "String",
    "pinRequired": "Boolean",
    "pinRequiredInsteadOfBiometricTimeout": "String (duration)",
    "previousPinBlockCount": "Integer",
    "printBlocked": "Boolean",
    "saveAsBlocked": "Boolean",
    "simplePinBlocked": "Boolean",
    "allowedAndroidDeviceManufacturers": "String",
    "allowedAndroidDeviceModels": [
      "String"
    ],
    "allowedIosDeviceModels": "String",
    "appActionIfAndroidDeviceManufacturerNotAllowed": "String",
    "appActionIfAndroidDeviceModelNotAllowed": "String",
    "appActionIfAndroidSafetyNetAppsVerificationFailed": "String",
    "appActionIfAndroidSafetyNetDeviceAttestationFailed": "String",
    "appActionIfDeviceLockNotSet": "String",
    "appActionIfIosDeviceModelNotAllowed": "String",
    "appDataEncryptionType": "String",
    "biometricAuthenticationBlocked": "Boolean",
    "blockAfterCompanyPortalUpdateDeferralInDays": "Integer",
    "customBrowserDisplayName": "String",
    "customBrowserPackageId": "String",
    "customBrowserProtocol": "String",
    "customDialerAppDisplayName": "String",
    "customDialerAppPackageId": "String",
    "customDialerAppProtocol": "String",
    "customSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "deployedAppCount": "Integer",
    "deviceLockRequired": "Boolean",
    "disableAppEncryptionIfDeviceEncryptionIsEnabled": "Boolean",
    "disableProtectionOfManagedOutboundOpenInData": "Boolean",
    "encryptAppData": "Boolean",
    "exemptedAppPackages": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "exemptedAppProtocols": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "faceIdBlocked": "Boolean",
    "filterOpenInToOnlyManagedApps": "Boolean",
    "minimumRequiredCompanyPortalVersion": "String",
    "minimumRequiredPatchVersion": "String",
    "minimumRequiredSdkVersion": "String",
    "minimumWarningCompanyPortalVersion": "String",
    "minimumWarningPatchVersion": "String",
    "minimumWipeCompanyPortalVersion": "String",
    "minimumWipePatchVersion": "String",
    "minimumWipeSdkVersion": "String",
    "protectInboundDataFromUnknownSources": "Boolean",
    "requiredAndroidSafetyNetAppsVerificationType": "String",
    "requiredAndroidSafetyNetDeviceAttestationType": "String",
    "requiredAndroidSafetyNetEvaluationType": "String",
    "screenCaptureBlocked": "Boolean",
    "thirdPartyKeyboardsBlocked": "Boolean",
    "warnAfterCompanyPortalUpdateDeferralInDays": "Integer",
    "wipeAfterCompanyPortalUpdateDeferralInDays": "Integer"
  }
}
```


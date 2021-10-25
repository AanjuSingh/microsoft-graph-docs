---
title: "Get androidDeviceOwnerGeneralDeviceConfiguration"
description: "Read the properties and relationships of an androidDeviceOwnerGeneralDeviceConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get androidDeviceOwnerGeneralDeviceConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [androidDeviceOwnerGeneralDeviceConfiguration](../resources/androiddeviceownergeneraldeviceconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration not found
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

If successful, this method returns a `200 OK` response code and an [androidDeviceOwnerGeneralDeviceConfiguration](../resources/androiddeviceownergeneraldeviceconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_androiddeviceownergeneraldeviceconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerGeneralDeviceConfiguration",
    "id": "b5e2d985-d985-b5e2-85d9-e2b585d9e2b5",
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
    "accountsBlockModification": "Boolean",
    "appsAllowInstallFromUnknownSources": "Boolean",
    "appsAutoUpdatePolicy": "String",
    "appsDefaultPermissionPolicy": "String",
    "appsRecommendSkippingFirstUseHints": "Boolean",
    "azureAdSharedDeviceDataClearApps": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "bluetoothBlockConfiguration": "Boolean",
    "bluetoothBlockContactSharing": "Boolean",
    "cameraBlocked": "Boolean",
    "cellularBlockWiFiTethering": "Boolean",
    "certificateCredentialConfigurationDisabled": "Boolean",
    "dataRoamingBlocked": "Boolean",
    "dateTimeConfigurationBlocked": "Boolean",
    "enrollmentProfile": "String",
    "factoryResetBlocked": "Boolean",
    "factoryResetDeviceAdministratorEmails": [
      "String"
    ],
    "globalProxy": {
      "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxy"
    },
    "googleAccountsBlocked": "Boolean",
    "kioskCustomizationDeviceSettingsBlocked": "Boolean",
    "kioskCustomizationPowerButtonActionsBlocked": "Boolean",
    "kioskCustomizationStatusBar": "String",
    "kioskCustomizationSystemErrorWarnings": "Boolean",
    "kioskCustomizationSystemNavigation": "String",
    "kioskModeAppOrderEnabled": "Boolean",
    "kioskModeAppPositions": [
      {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
      }
    ],
    "kioskModeApps": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "kioskModeAppsInFolderOrderedByName": "Boolean",
    "kioskModeBluetoothConfigurationEnabled": "Boolean",
    "kioskModeDebugMenuEasyAccessEnabled": "Boolean",
    "kioskModeExitCode": "String",
    "kioskModeFlashlightConfigurationEnabled": "Boolean",
    "kioskModeFolderIcon": "String",
    "kioskModeGridHeight": "Integer",
    "kioskModeGridWidth": "Integer",
    "kioskModeIconSize": "String",
    "kioskModeLockHomeScreen": "Boolean",
    "kioskModeManagedFolders": [
      {
        "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeManagedFolder"
      }
    ],
    "kioskModeManagedHomeScreenAutoSignout": "Boolean",
    "kioskModeManagedHomeScreenInactiveSignOutDelayInSeconds": "Integer",
    "kioskModeManagedHomeScreenInactiveSignOutNoticeInSeconds": "Integer",
    "kioskModeManagedHomeScreenPinComplexity": "String",
    "kioskModeManagedHomeScreenPinRequired": "Boolean",
    "kioskModeManagedHomeScreenPinRequiredToResume": "Boolean",
    "kioskModeManagedHomeScreenSignInBackground": "String",
    "kioskModeManagedHomeScreenSignInBrandingLogo": "String",
    "kioskModeManagedHomeScreenSignInEnabled": "Boolean",
    "kioskModeManagedSettingsEntryDisabled": "Boolean",
    "kioskModeMediaVolumeConfigurationEnabled": "Boolean",
    "kioskModeScreenOrientation": "String",
    "kioskModeScreenSaverConfigurationEnabled": "Boolean",
    "kioskModeScreenSaverDetectMediaDisabled": "Boolean",
    "kioskModeScreenSaverDisplayTimeInSeconds": "Integer",
    "kioskModeScreenSaverImageUrl": "String",
    "kioskModeScreenSaverStartDelayInSeconds": "Integer",
    "kioskModeShowAppNotificationBadge": "Boolean",
    "kioskModeShowDeviceInfo": "Boolean",
    "kioskModeVirtualHomeButtonEnabled": "Boolean",
    "kioskModeVirtualHomeButtonType": "String",
    "kioskModeWallpaperUrl": "String",
    "kioskModeWifiAllowedSsids": [
      "String"
    ],
    "kioskModeWiFiConfigurationEnabled": "Boolean",
    "microphoneForceMute": "Boolean",
    "microsoftLauncherConfigurationEnabled": "Boolean",
    "microsoftLauncherCustomWallpaperAllowUserModification": "Boolean",
    "microsoftLauncherCustomWallpaperEnabled": "Boolean",
    "microsoftLauncherCustomWallpaperImageUrl": "String",
    "microsoftLauncherDockPresenceAllowUserModification": "Boolean",
    "microsoftLauncherDockPresenceConfiguration": "String",
    "microsoftLauncherFeedAllowUserModification": "Boolean",
    "microsoftLauncherFeedEnabled": "Boolean",
    "microsoftLauncherSearchBarPlacementConfiguration": "String",
    "networkEscapeHatchAllowed": "Boolean",
    "nfcBlockOutgoingBeam": "Boolean",
    "passwordBlockKeyguard": "Boolean",
    "passwordBlockKeyguardFeatures": [
      "String"
    ],
    "passwordExpirationDays": "Integer",
    "passwordMinimumLength": "Integer",
    "passwordMinimumLetterCharacters": "Integer",
    "passwordMinimumLowerCaseCharacters": "Integer",
    "passwordMinimumNonLetterCharacters": "Integer",
    "passwordMinimumNumericCharacters": "Integer",
    "passwordMinimumSymbolCharacters": "Integer",
    "passwordMinimumUpperCaseCharacters": "Integer",
    "passwordMinutesOfInactivityBeforeScreenTimeout": "Integer",
    "passwordPreviousPasswordCountToBlock": "Integer",
    "passwordRequiredType": "String",
    "passwordSignInFailureCountBeforeFactoryReset": "Integer",
    "personalProfileAppsAllowInstallFromUnknownSources": "Boolean",
    "personalProfileCameraBlocked": "Boolean",
    "personalProfilePersonalApplications": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "personalProfilePlayStoreMode": "String",
    "personalProfileScreenCaptureBlocked": "Boolean",
    "playStoreMode": "String",
    "safeBootBlocked": "Boolean",
    "screenCaptureBlocked": "Boolean",
    "securityAllowDebuggingFeatures": "Boolean",
    "securityDeveloperSettingsEnabled": "Boolean",
    "securityRequireVerifyApps": "Boolean",
    "statusBarBlocked": "Boolean",
    "stayOnModes": [
      "String"
    ],
    "storageAllowUsb": "Boolean",
    "storageBlockExternalMedia": "Boolean",
    "storageBlockUsbFileTransfer": "Boolean",
    "systemUpdateInstallType": "String",
    "systemUpdateWindowEndMinutesAfterMidnight": "Integer",
    "systemUpdateWindowStartMinutesAfterMidnight": "Integer",
    "systemWindowsBlocked": "Boolean",
    "usersBlockAdd": "Boolean",
    "usersBlockRemove": "Boolean",
    "volumeBlockAdjustment": "Boolean",
    "vpnAlwaysOnLockdownMode": "Boolean",
    "vpnAlwaysOnPackageIdentifier": "String",
    "wifiBlockEditConfigurations": "Boolean",
    "wifiBlockEditPolicyDefinedConfigurations": "Boolean",
    "workProfilePasswordExpirationDays": "Integer",
    "workProfilePasswordMinimumLength": "Integer",
    "workProfilePasswordMinimumLetterCharacters": "Integer",
    "workProfilePasswordMinimumLowerCaseCharacters": "Integer",
    "workProfilePasswordMinimumNonLetterCharacters": "Integer",
    "workProfilePasswordMinimumNumericCharacters": "Integer",
    "workProfilePasswordMinimumSymbolCharacters": "Integer",
    "workProfilePasswordMinimumUpperCaseCharacters": "Integer",
    "workProfilePasswordPreviousPasswordCountToBlock": "Integer",
    "workProfilePasswordRequiredType": "String",
    "workProfilePasswordSignInFailureCountBeforeFactoryReset": "Integer"
  }
}
```


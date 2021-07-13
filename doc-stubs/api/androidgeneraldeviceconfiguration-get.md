---
title: "Get androidGeneralDeviceConfiguration"
description: "Read the properties and relationships of an androidGeneralDeviceConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get androidGeneralDeviceConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.androidGeneralDeviceConfiguration not found
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

If successful, this method returns a `200 OK` response code and an [androidGeneralDeviceConfiguration](../resources/androidgeneraldeviceconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_androidgeneraldeviceconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.androidGeneralDeviceConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.androidGeneralDeviceConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.androidGeneralDeviceConfiguration",
    "id": "7df7a879-a879-7df7-79a8-f77d79a8f77d",
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
    "appsBlockClipboardSharing": "Boolean",
    "appsBlockCopyPaste": "Boolean",
    "appsBlockYouTube": "Boolean",
    "appsHideList": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "appsInstallAllowList": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "appsLaunchBlockList": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "bluetoothBlocked": "Boolean",
    "cameraBlocked": "Boolean",
    "cellularBlockDataRoaming": "Boolean",
    "cellularBlockMessaging": "Boolean",
    "cellularBlockVoiceRoaming": "Boolean",
    "cellularBlockWiFiTethering": "Boolean",
    "compliantAppListType": "String",
    "compliantAppsList": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "dateAndTimeBlockChanges": "Boolean",
    "deviceSharingAllowed": "Boolean",
    "diagnosticDataBlockSubmission": "Boolean",
    "factoryResetBlocked": "Boolean",
    "googleAccountBlockAutoSync": "Boolean",
    "googlePlayStoreBlocked": "Boolean",
    "kioskModeApps": [
      {
        "@odata.type": "microsoft.graph.appListItem"
      }
    ],
    "kioskModeBlockSleepButton": "Boolean",
    "kioskModeBlockVolumeButtons": "Boolean",
    "locationServicesBlocked": "Boolean",
    "nfcBlocked": "Boolean",
    "passwordBlockFingerprintUnlock": "Boolean",
    "passwordBlockTrustAgents": "Boolean",
    "passwordExpirationDays": "Integer",
    "passwordMinimumLength": "Integer",
    "passwordMinutesOfInactivityBeforeScreenTimeout": "Integer",
    "passwordPreviousPasswordBlockCount": "Integer",
    "passwordRequired": "Boolean",
    "passwordRequiredType": "String",
    "passwordSignInFailureCountBeforeFactoryReset": "Integer",
    "powerOffBlocked": "Boolean",
    "requiredPasswordComplexity": "String",
    "screenCaptureBlocked": "Boolean",
    "securityRequireVerifyApps": "Boolean",
    "storageBlockGoogleBackup": "Boolean",
    "storageBlockRemovableStorage": "Boolean",
    "storageRequireDeviceEncryption": "Boolean",
    "storageRequireRemovableStorageEncryption": "Boolean",
    "voiceAssistantBlocked": "Boolean",
    "voiceDialingBlocked": "Boolean",
    "webBrowserBlockAutofill": "Boolean",
    "webBrowserBlocked": "Boolean",
    "webBrowserBlockJavaScript": "Boolean",
    "webBrowserBlockPopups": "Boolean",
    "webBrowserCookieSettings": "String",
    "wiFiBlocked": "Boolean"
  }
}
```


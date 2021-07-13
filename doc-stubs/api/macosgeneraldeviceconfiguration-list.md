---
title: "List macOSGeneralDeviceConfigurations"
description: "Get a list of the macOSGeneralDeviceConfiguration objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List macOSGeneralDeviceConfigurations
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [macOSGeneralDeviceConfiguration](../resources/macosgeneraldeviceconfiguration.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.macOSGeneralDeviceConfiguration not found
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

If successful, this method returns a `200 OK` response code and a collection of [macOSGeneralDeviceConfiguration](../resources/macosgeneraldeviceconfiguration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_macosgeneraldeviceconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.macOSGeneralDeviceConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.macOSGeneralDeviceConfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
      "id": "8b319244-9244-8b31-4492-318b4492318b",
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
      "airDropBlocked": "Boolean",
      "airPrintBlocked": "Boolean",
      "airPrintBlockiBeaconDiscovery": "Boolean",
      "airPrintForceTrustedTLS": "Boolean",
      "appleWatchBlockAutoUnlock": "Boolean",
      "cameraBlocked": "Boolean",
      "classroomAppBlockRemoteScreenObservation": "Boolean",
      "classroomAppForceUnpromptedScreenObservation": "Boolean",
      "classroomForceAutomaticallyJoinClasses": "Boolean",
      "classroomForceRequestPermissionToLeaveClasses": "Boolean",
      "classroomForceUnpromptedAppAndDeviceLock": "Boolean",
      "compliantAppListType": "String",
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem"
        }
      ],
      "contentCachingBlocked": "Boolean",
      "definitionLookupBlocked": "Boolean",
      "emailInDomainSuffixes": [
        "String"
      ],
      "iCloudBlockActivityContinuation": "Boolean",
      "iCloudBlockAddressBook": "Boolean",
      "iCloudBlockBookmarks": "Boolean",
      "iCloudBlockCalendar": "Boolean",
      "iCloudBlockDocumentSync": "Boolean",
      "iCloudBlockMail": "Boolean",
      "iCloudBlockNotes": "Boolean",
      "iCloudBlockPhotoLibrary": "Boolean",
      "iCloudBlockReminders": "Boolean",
      "iTunesBlockFileSharing": "Boolean",
      "iTunesBlockMusicService": "Boolean",
      "keyboardBlockDictation": "Boolean",
      "keychainBlockCloudSync": "Boolean",
      "passwordBlockAirDropSharing": "Boolean",
      "passwordBlockAutoFill": "Boolean",
      "passwordBlockFingerprintUnlock": "Boolean",
      "passwordBlockModification": "Boolean",
      "passwordBlockProximityRequests": "Boolean",
      "passwordBlockSimple": "Boolean",
      "passwordExpirationDays": "Integer",
      "passwordMaximumAttemptCount": "Integer",
      "passwordMinimumCharacterSetCount": "Integer",
      "passwordMinimumLength": "Integer",
      "passwordMinutesOfInactivityBeforeLock": "Integer",
      "passwordMinutesOfInactivityBeforeScreenTimeout": "Integer",
      "passwordMinutesUntilFailedLoginReset": "Integer",
      "passwordPreviousPasswordBlockCount": "Integer",
      "passwordRequired": "Boolean",
      "passwordRequiredType": "String",
      "privacyAccessControls": [
        {
          "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem"
        }
      ],
      "safariBlockAutofill": "Boolean",
      "screenCaptureBlocked": "Boolean",
      "softwareUpdatesEnforcedDelayInDays": "Integer",
      "spotlightBlockInternetResults": "Boolean",
      "updateDelayPolicy": "String"
    }
  ]
}
```


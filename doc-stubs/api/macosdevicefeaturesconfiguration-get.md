---
title: "Get macOSDeviceFeaturesConfiguration"
description: "Read the properties and relationships of a macOSDeviceFeaturesConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get macOSDeviceFeaturesConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.macOSDeviceFeaturesConfiguration not found
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

If successful, this method returns a `200 OK` response code and a [macOSDeviceFeaturesConfiguration](../resources/macosdevicefeaturesconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_macosdevicefeaturesconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.macOSDeviceFeaturesConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.macOSDeviceFeaturesConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
    "id": "50e462e5-62e5-50e4-e562-e450e562e450",
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
    "airPrintDestinations": [
      {
        "@odata.type": "microsoft.graph.airPrintDestination"
      }
    ],
    "adminShowHostInfo": "Boolean",
    "appAssociatedDomains": [
      {
        "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
      }
    ],
    "associatedDomains": [
      {
        "@odata.type": "microsoft.graph.keyValuePair"
      }
    ],
    "authorizedUsersListHidden": "Boolean",
    "authorizedUsersListHideAdminUsers": "Boolean",
    "authorizedUsersListHideLocalUsers": "Boolean",
    "authorizedUsersListHideMobileAccounts": "Boolean",
    "authorizedUsersListIncludeNetworkUsers": "Boolean",
    "authorizedUsersListShowOtherManagedUsers": "Boolean",
    "autoLaunchItems": [
      {
        "@odata.type": "microsoft.graph.macOSLaunchItem"
      }
    ],
    "consoleAccessDisabled": "Boolean",
    "contentCachingBlockDeletion": "Boolean",
    "contentCachingClientListenRanges": [
      {
        "@odata.type": "microsoft.graph.iPv4CidrRange"
      }
    ],
    "contentCachingClientPolicy": "String",
    "contentCachingDataPath": "String",
    "contentCachingDisableConnectionSharing": "Boolean",
    "contentCachingEnabled": "Boolean",
    "contentCachingForceConnectionSharing": "Boolean",
    "contentCachingKeepAwake": "Boolean",
    "contentCachingLogClientIdentities": "Boolean",
    "contentCachingMaxSizeBytes": "Integer",
    "contentCachingParents": [
      "String"
    ],
    "contentCachingParentSelectionPolicy": "String",
    "contentCachingPeerFilterRanges": [
      {
        "@odata.type": "microsoft.graph.iPv4CidrRange"
      }
    ],
    "contentCachingPeerListenRanges": [
      {
        "@odata.type": "microsoft.graph.iPv4CidrRange"
      }
    ],
    "contentCachingPeerPolicy": "String",
    "contentCachingPort": "Integer",
    "contentCachingPublicRanges": [
      {
        "@odata.type": "microsoft.graph.iPv4CidrRange"
      }
    ],
    "contentCachingShowAlerts": "Boolean",
    "contentCachingType": "String",
    "loginWindowText": "String",
    "logOutDisabledWhileLoggedIn": "Boolean",
    "macOSSingleSignOnExtension": {
      "@odata.type": "microsoft.graph.macOSSingleSignOnExtension"
    },
    "powerOffDisabledWhileLoggedIn": "Boolean",
    "restartDisabled": "Boolean",
    "restartDisabledWhileLoggedIn": "Boolean",
    "screenLockDisableImmediate": "Boolean",
    "shutDownDisabled": "Boolean",
    "shutDownDisabledWhileLoggedIn": "Boolean",
    "singleSignOnExtension": {
      "@odata.type": "microsoft.graph.singleSignOnExtension"
    },
    "sleepDisabled": "Boolean"
  }
}
```


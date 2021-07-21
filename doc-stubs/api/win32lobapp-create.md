---
title: "Create win32LobApp"
description: "Create a new win32LobApp object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create win32LobApp
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [win32LobApp](../resources/win32lobapp.md) object.

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
POST ** Collection URI for microsoft.graph.win32LobApp not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [win32LobApp](../resources/win32lobapp.md) object.

The following table shows the properties that are required when you create the [win32LobApp](../resources/win32lobapp.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md)|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/mobileapp.md)|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/mobileapp.md)|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md)|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md)|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md)|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md)|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md)|
|publishingState|mobileAppPublishingState|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|supersededAppCount|Int32|The total number of apps this app is directly or indirectly superseded by. Inherited from [mobileApp](../resources/mobileapp.md)|
|supersedingAppCount|Int32|The total number of apps this app directly or indirectly supersedes. Inherited from [mobileApp](../resources/mobileapp.md)|
|uploadState|Int32|The upload state. Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Inherited from [mobileApp](../resources/mobileapp.md)|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|applicableArchitectures|windowsArchitecture|The Windows architecture(s) for which this app can run on. Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|detectionRules|[win32LobAppDetection](../resources/win32lobappdetection.md) collection|The detection rules to detect Win32 Line of Business (LoB) app.|
|displayVersion|String|The version displayed in the UX for this app.|
|installCommandLine|String|The command line to install this app|
|installExperience|[win32LobAppInstallExperience](../resources/win32lobappinstallexperience.md)|The install experience for this app.|
|minimumCpuSpeedInMHz|Int32|The value for the minimum CPU speed which is required to install this app.|
|minimumFreeDiskSpaceInMB|Int32|The value for the minimum free disk space which is required to install this app.|
|minimumMemoryInMB|Int32|The value for the minimum physical memory which is required to install this app.|
|minimumNumberOfProcessors|Int32|The value for the minimum number of processors which is required to install this app.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/windowsminimumoperatingsystem.md)|The value for the minimum applicable operating system.|
|minimumSupportedWindowsRelease|String|The value for the minimum supported windows release.|
|msiInformation|[win32LobAppMsiInformation](../resources/win32lobappmsiinformation.md)|The MSI details if this Win32 app is an MSI app.|
|requirementRules|[win32LobAppRequirement](../resources/win32lobapprequirement.md) collection|The requirement rules to detect Win32 Line of Business (LoB) app.|
|returnCodes|[win32LobAppReturnCode](../resources/win32lobappreturncode.md) collection|The return codes for post installation behavior.|
|rules|[win32LobAppRule](../resources/win32lobapprule.md) collection|The detection and requirement rules for this app.|
|setupFilePath|String|The relative path of the setup file in the encrypted Win32LobApp package.|
|uninstallCommandLine|String|The command line to uninstall this app|



## Response

If successful, this method returns a `201 Created` response code and a [win32LobApp](../resources/win32lobapp.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_win32lobapp_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.win32LobApp not found
Content-Type: application/json
Content-length: 1822

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "dependentAppCount": "Integer",
  "description": "String",
  "developer": "String",
  "displayName": "String",
  "informationUrl": "String",
  "isAssigned": "Boolean",
  "isFeatured": "Boolean",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "notes": "String",
  "owner": "String",
  "privacyInformationUrl": "String",
  "publisher": "String",
  "publishingState": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "supersededAppCount": "Integer",
  "supersedingAppCount": "Integer",
  "uploadState": "Integer",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": "Integer",
  "applicableArchitectures": "String",
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
    }
  ],
  "displayVersion": "String",
  "installCommandLine": "String",
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
  },
  "minimumCpuSpeedInMHz": "Integer",
  "minimumFreeDiskSpaceInMB": "Integer",
  "minimumMemoryInMB": "Integer",
  "minimumNumberOfProcessors": "Integer",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
  },
  "minimumSupportedWindowsRelease": "String",
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
  },
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
    }
  ],
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
    }
  ],
  "setupFilePath": "String",
  "uninstallCommandLine": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.win32LobApp"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "8a3d6aba-6aba-8a3d-ba6a-3d8aba6a3d8a",
  "createdDateTime": "String (timestamp)",
  "dependentAppCount": "Integer",
  "description": "String",
  "developer": "String",
  "displayName": "String",
  "informationUrl": "String",
  "isAssigned": "Boolean",
  "isFeatured": "Boolean",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "notes": "String",
  "owner": "String",
  "privacyInformationUrl": "String",
  "publisher": "String",
  "publishingState": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "supersededAppCount": "Integer",
  "supersedingAppCount": "Integer",
  "uploadState": "Integer",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": "Integer",
  "applicableArchitectures": "String",
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
    }
  ],
  "displayVersion": "String",
  "installCommandLine": "String",
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience"
  },
  "minimumCpuSpeedInMHz": "Integer",
  "minimumFreeDiskSpaceInMB": "Integer",
  "minimumMemoryInMB": "Integer",
  "minimumNumberOfProcessors": "Integer",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
  },
  "minimumSupportedWindowsRelease": "String",
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation"
  },
  "requirementRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppFileSystemRequirement"
    }
  ],
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode"
    }
  ],
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppFileSystemRule"
    }
  ],
  "setupFilePath": "String",
  "uninstallCommandLine": "String"
}
```


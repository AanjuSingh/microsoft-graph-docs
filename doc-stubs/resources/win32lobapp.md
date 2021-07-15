---
title: "win32LobApp resource type"
description: "Contains properties and inherited properties for Win32 apps."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# win32LobApp resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties and inherited properties for Win32 apps.


Inherits from [mobileLobApp](../resources/mobilelobapp.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List win32LobApp](../api/win32lobapp-list.md)|[win32LobApp](../resources/win32lobapp.md) collection|Get a list of the [win32LobApp](../resources/win32lobapp.md) objects and their properties.|
|[Create win32LobApp](../api/win32lobapp-create.md)|[win32LobApp](../resources/win32lobapp.md)|Create a new [win32LobApp](../resources/win32lobapp.md) object.|
|[Get win32LobApp](../api/win32lobapp-get.md)|[win32LobApp](../resources/win32lobapp.md)|Read the properties and relationships of a [win32LobApp](../resources/win32lobapp.md) object.|
|[Update win32LobApp](../api/win32lobapp-update.md)|[win32LobApp](../resources/win32lobapp.md)|Update the properties of a [win32LobApp](../resources/win32lobapp.md) object.|
|[Delete win32LobApp](../api/win32lobapp-delete.md)|None|Deletes a [win32LobApp](../resources/win32lobapp.md) object.|
|[List assignments](../api/win32lobapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignment resources from the assignments navigation property.|
|[Create mobileAppAssignment](../api/win32lobapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Create a new mobileAppAssignment object.|
|[List categories](../api/win32lobapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategory resources from the categories navigation property.|
|[Add mobileAppCategory](../api/win32lobapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Add categories by posting to the categories collection.|
|[List contentVersions](../api/win32lobapp-list-contentversions.md)|[mobileAppContent](../resources/mobileappcontent.md) collection|Get the mobileAppContent resources from the contentVersions navigation property.|
|[Create mobileAppContent](../api/win32lobapp-post-contentversions.md)|[mobileAppContent](../resources/mobileappcontent.md)|Create a new mobileAppContent object.|
|[List deviceStatuses](../api/win32lobapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatus resources from the deviceStatuses navigation property.|
|[Create mobileAppInstallStatus](../api/win32lobapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Create a new mobileAppInstallStatus object.|
|[List mobileAppInstallSummary](../api/win32lobapp-list-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md) collection|Get the mobileAppInstallSummary resources from the installSummary navigation property.|
|[Create mobileAppInstallSummary](../api/win32lobapp-post-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Create a new mobileAppInstallSummary object.|
|[List relationships](../api/win32lobapp-list-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|Get the mobileAppRelationship resources from the relationships navigation property.|
|[Create mobileAppRelationship](../api/win32lobapp-post-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md)|Create a new mobileAppRelationship object.|
|[List userStatuses](../api/win32lobapp-list-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|Get the userAppInstallStatus resources from the userStatuses navigation property.|
|[Create userAppInstallStatus](../api/win32lobapp-post-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Create a new userAppInstallStatus object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applicableArchitectures|windowsArchitecture|The Windows architecture(s) for which this app can run on. Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.|
|committedContentVersion|String|The internal committed content version. Inherited from [mobileLobApp](../resources/mobilelobapp.md).|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md).|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/mobileapp.md).|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|detectionRules|[win32LobAppDetection](../resources/win32lobappdetection.md) collection|The detection rules to detect Win32 Line of Business (LoB) app.|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|displayVersion|String|The version displayed in the UX for this app.|
|fileName|String|The name of the main Lob application file. Inherited from [mobileLobApp](../resources/mobilelobapp.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md).|
|installCommandLine|String|The command line to install this app|
|installExperience|[win32LobAppInstallExperience](../resources/win32lobappinstallexperience.md)|The install experience for this app.|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/mobileapp.md).|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md).|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md).|
|minimumCpuSpeedInMHz|Int32|The value for the minimum CPU speed which is required to install this app.|
|minimumFreeDiskSpaceInMB|Int32|The value for the minimum free disk space which is required to install this app.|
|minimumMemoryInMB|Int32|The value for the minimum physical memory which is required to install this app.|
|minimumNumberOfProcessors|Int32|The value for the minimum number of processors which is required to install this app.|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/windowsminimumoperatingsystem.md)|The value for the minimum applicable operating system.|
|minimumSupportedWindowsRelease|String|The value for the minimum supported windows release.|
|msiInformation|[win32LobAppMsiInformation](../resources/win32lobappmsiinformation.md)|The MSI details if this Win32 app is an MSI app.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md).|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|publishingState|mobileAppPublishingState|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|requirementRules|[win32LobAppRequirement](../resources/win32lobapprequirement.md) collection|The requirement rules to detect Win32 Line of Business (LoB) app.|
|returnCodes|[win32LobAppReturnCode](../resources/win32lobappreturncode.md) collection|The return codes for post installation behavior.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md).|
|rules|[win32LobAppRule](../resources/win32lobapprule.md) collection|The detection and requirement rules for this app.|
|setupFilePath|String|The relative path of the setup file in the encrypted Win32LobApp package.|
|size|Int64|The total size, including all uploaded files. Inherited from [mobileLobApp](../resources/mobilelobapp.md).|
|supersededAppCount|Int32|The total number of apps this app is directly or indirectly superseded by. Inherited from [mobileApp](../resources/mobileapp.md).|
|supersedingAppCount|Int32|The total number of apps this app directly or indirectly supersedes. Inherited from [mobileApp](../resources/mobileapp.md).|
|uninstallCommandLine|String|The command line to uninstall this app|
|uploadState|Int32|The upload state. Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Inherited from [mobileApp](../resources/mobileapp.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/mobileappcontent.md) collection|The list of content versions for this app. Inherited from [mobileLobApp](../resources/mobilelobapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|The set of direct relationships for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.win32LobApp",
  "baseType": "microsoft.graph.mobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "String (identifier)",
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


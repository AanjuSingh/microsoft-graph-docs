---
title: "managedAndroidLobApp resource type"
description: "Contains properties and inherited properties for Managed Android Line Of Business apps."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAndroidLobApp resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties and inherited properties for Managed Android Line Of Business apps.


Inherits from [managedMobileLobApp](../resources/managedmobilelobapp.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedAndroidLobApps](../api/managedandroidlobapp-list.md)|[managedAndroidLobApp](../resources/managedandroidlobapp.md) collection|Get a list of the [managedAndroidLobApp](../resources/managedandroidlobapp.md) objects and their properties.|
|[Create managedAndroidLobApp](../api/managedandroidlobapp-create.md)|[managedAndroidLobApp](../resources/managedandroidlobapp.md)|Create a new [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[Get managedAndroidLobApp](../api/managedandroidlobapp-get.md)|[managedAndroidLobApp](../resources/managedandroidlobapp.md)|Read the properties and relationships of a [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[Update managedAndroidLobApp](../api/managedandroidlobapp-update.md)|[managedAndroidLobApp](../resources/managedandroidlobapp.md)|Update the properties of a [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[Delete managedAndroidLobApp](../api/managedandroidlobapp-delete.md)|None|Deletes a [managedAndroidLobApp](../resources/managedandroidlobapp.md) object.|
|[List assignments](../api/managedandroidlobapp-list-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md) collection|Get the mobileAppAssignment resources from the assignments navigation property.|
|[Create mobileAppAssignment](../api/managedandroidlobapp-post-assignments.md)|[mobileAppAssignment](../resources/mobileappassignment.md)|Create a new mobileAppAssignment object.|
|[List categories](../api/managedandroidlobapp-list-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md) collection|Get the mobileAppCategory resources from the categories navigation property.|
|[Add mobileAppCategory](../api/managedandroidlobapp-post-categories.md)|[mobileAppCategory](../resources/mobileappcategory.md)|Add categories by posting to the categories collection.|
|[List contentVersions](../api/managedandroidlobapp-list-contentversions.md)|[mobileAppContent](../resources/mobileappcontent.md) collection|Get the mobileAppContent resources from the contentVersions navigation property.|
|[Create mobileAppContent](../api/managedandroidlobapp-post-contentversions.md)|[mobileAppContent](../resources/mobileappcontent.md)|Create a new mobileAppContent object.|
|[List deviceStatuses](../api/managedandroidlobapp-list-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|Get the mobileAppInstallStatus resources from the deviceStatuses navigation property.|
|[Create mobileAppInstallStatus](../api/managedandroidlobapp-post-devicestatuses.md)|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md)|Create a new mobileAppInstallStatus object.|
|[List mobileAppInstallSummary](../api/managedandroidlobapp-list-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md) collection|Get the mobileAppInstallSummary resources from the installSummary navigation property.|
|[Create mobileAppInstallSummary](../api/managedandroidlobapp-post-installsummary.md)|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Create a new mobileAppInstallSummary object.|
|[List relationships](../api/managedandroidlobapp-list-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|Get the mobileAppRelationship resources from the relationships navigation property.|
|[Create mobileAppRelationship](../api/managedandroidlobapp-post-relationships.md)|[mobileAppRelationship](../resources/mobileapprelationship.md)|Create a new mobileAppRelationship object.|
|[List userStatuses](../api/managedandroidlobapp-list-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|Get the userAppInstallStatus resources from the userStatuses navigation property.|
|[Create userAppInstallStatus](../api/managedandroidlobapp-post-userstatuses.md)|[userAppInstallStatus](../resources/userappinstallstatus.md)|Create a new userAppInstallStatus object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appAvailability|managedAppAvailability|The Application's availability. Inherited from [managedApp](../resources/managedapp.md). Possible values are: `global`, `lineOfBusiness`.|
|committedContentVersion|String|The internal committed content version. Inherited from [managedMobileLobApp](../resources/managedmobilelobapp.md).|
|createdDateTime|DateTimeOffset|The date and time the app was created. Inherited from [mobileApp](../resources/mobileapp.md).|
|dependentAppCount|Int32|The total number of dependencies the child app has. Inherited from [mobileApp](../resources/mobileapp.md).|
|description|String|The description of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|developer|String|The developer of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|displayName|String|The admin provided or imported title of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|fileName|String|The name of the main Lob application file. Inherited from [managedMobileLobApp](../resources/managedmobilelobapp.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|identityName|String|The Identity Name.|
|identityVersion|String|The identity version.|
|informationUrl|String|The more information Url. Inherited from [mobileApp](../resources/mobileapp.md).|
|isAssigned|Boolean|The value indicating whether the app is assigned to at least one group. Inherited from [mobileApp](../resources/mobileapp.md).|
|isFeatured|Boolean|The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/mobileapp.md).|
|largeIcon|[mimeContent](../resources/mimecontent.md)|The large icon, to be displayed in the app details and used for upload of the icon. Inherited from [mobileApp](../resources/mobileapp.md).|
|lastModifiedDateTime|DateTimeOffset|The date and time the app was last modified. Inherited from [mobileApp](../resources/mobileapp.md).|
|minimumSupportedOperatingSystem|[androidMinimumOperatingSystem](../resources/androidminimumoperatingsystem.md)|The value for the minimum applicable operating system.|
|notes|String|Notes for the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|owner|String|The owner of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|packageId|String|The package identifier.|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [mobileApp](../resources/mobileapp.md).|
|publisher|String|The publisher of the app. Inherited from [mobileApp](../resources/mobileapp.md).|
|publishingState|mobileAppPublishingState|The publishing state for the app. The app cannot be assigned unless the app is published. Inherited from [mobileApp](../resources/mobileapp.md). Possible values are: `notPublished`, `processing`, `published`.|
|roleScopeTagIds|String collection|List of scope tag ids for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md).|
|size|Int64|The total size, including all uploaded files. Inherited from [managedMobileLobApp](../resources/managedmobilelobapp.md).|
|supersededAppCount|Int32|The total number of apps this app is directly or indirectly superseded by. Inherited from [mobileApp](../resources/mobileapp.md).|
|supersedingAppCount|Int32|The total number of apps this app directly or indirectly supersedes. Inherited from [mobileApp](../resources/mobileapp.md).|
|uploadState|Int32|The upload state. Possible values are: 0 - `Not Ready`, 1 - `Ready`, 2 - `Processing`. Inherited from [mobileApp](../resources/mobileapp.md).|
|version|String|The Application's version. Inherited from [managedApp](../resources/managedapp.md).|
|versionCode|String|The version code of managed Android Line of Business (LoB) app.|
|versionName|String|The version name of managed Android Line of Business (LoB) app.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[mobileAppAssignment](../resources/mobileappassignment.md) collection|The list of group assignments for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|categories|[mobileAppCategory](../resources/mobileappcategory.md) collection|The list of categories for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|contentVersions|[mobileAppContent](../resources/mobileappcontent.md) collection|The list of content versions for this app. Inherited from [managedMobileLobApp](../resources/managedmobilelobapp.md)|
|deviceStatuses|[mobileAppInstallStatus](../resources/mobileappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|
|installSummary|[mobileAppInstallSummary](../resources/mobileappinstallsummary.md)|Mobile App Install Summary. Inherited from [mobileApp](../resources/mobileapp.md)|
|relationships|[mobileAppRelationship](../resources/mobileapprelationship.md) collection|The set of direct relationships for this app. Inherited from [mobileApp](../resources/mobileapp.md)|
|userStatuses|[userAppInstallStatus](../resources/userappinstallstatus.md) collection|The list of installation states for this mobile app. Inherited from [mobileApp](../resources/mobileapp.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAndroidLobApp",
  "baseType": "microsoft.graph.managedMobileLobApp",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "appAvailability": "String",
  "version": "String",
  "committedContentVersion": "String",
  "fileName": "String",
  "size": "Integer",
  "identityName": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
  },
  "packageId": "String",
  "versionCode": "String",
  "versionName": "String"
}
```


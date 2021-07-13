---
title: "iosVppEBook resource type"
description: "A class containing the properties for iOS Vpp eBook."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosVppEBook resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A class containing the properties for iOS Vpp eBook.


Inherits from [managedEBook](../resources/managedebook.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List iosVppEBooks](../api/iosvppebook-list.md)|[iosVppEBook](../resources/iosvppebook.md) collection|Get a list of the [iosVppEBook](../resources/iosvppebook.md) objects and their properties.|
|[Create iosVppEBook](../api/iosvppebook-create.md)|[iosVppEBook](../resources/iosvppebook.md)|Create a new [iosVppEBook](../resources/iosvppebook.md) object.|
|[Get iosVppEBook](../api/iosvppebook-get.md)|[iosVppEBook](../resources/iosvppebook.md)|Read the properties and relationships of an [iosVppEBook](../resources/iosvppebook.md) object.|
|[Update iosVppEBook](../api/iosvppebook-update.md)|[iosVppEBook](../resources/iosvppebook.md)|Update the properties of an [iosVppEBook](../resources/iosvppebook.md) object.|
|[Delete iosVppEBook](../api/iosvppebook-delete.md)|None|Deletes an [iosVppEBook](../resources/iosvppebook.md) object.|
|[assign](../api/iosvppebook-assign.md)|None|**TODO: Add Description**|
|[List assignments](../api/iosvppebook-list-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md) collection|Get the managedEBookAssignment resources from the assignments navigation property.|
|[Create managedEBookAssignment](../api/iosvppebook-post-assignments.md)|[managedEBookAssignment](../resources/managedebookassignment.md)|Create a new managedEBookAssignment object.|
|[List categories](../api/iosvppebook-list-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md) collection|Get the managedEBookCategory resources from the categories navigation property.|
|[Add managedEBookCategory](../api/iosvppebook-post-categories.md)|[managedEBookCategory](../resources/managedebookcategory.md)|Add categories by posting to the categories collection.|
|[List deviceStates](../api/iosvppebook-list-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md) collection|Get the deviceInstallState resources from the deviceStates navigation property.|
|[Create deviceInstallState](../api/iosvppebook-post-devicestates.md)|[deviceInstallState](../resources/deviceinstallstate.md)|Create a new deviceInstallState object.|
|[List eBookInstallSummary](../api/iosvppebook-list-installsummary.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md) collection|Get the eBookInstallSummary resources from the installSummary navigation property.|
|[Create eBookInstallSummary](../api/iosvppebook-post-installsummary.md)|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Create a new eBookInstallSummary object.|
|[List userStateSummary](../api/iosvppebook-list-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|Get the userInstallStateSummary resources from the userStateSummary navigation property.|
|[Create userInstallStateSummary](../api/iosvppebook-post-userstatesummary.md)|[userInstallStateSummary](../resources/userinstallstatesummary.md)|Create a new userInstallStateSummary object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appleId|String|The Apple ID associated with Vpp token.|
|createdDateTime|DateTimeOffset|The date and time when the eBook file was created. Inherited from [managedEBook](../resources/managedebook.md).|
|description|String|Description. Inherited from [managedEBook](../resources/managedebook.md).|
|displayName|String|Name of the eBook. Inherited from [managedEBook](../resources/managedebook.md).|
|genres|String collection|Genres.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|informationUrl|String|The more information Url. Inherited from [managedEBook](../resources/managedebook.md).|
|language|String|Language.|
|largeCover|[mimeContent](../resources/mimecontent.md)|Book cover. Inherited from [managedEBook](../resources/managedebook.md).|
|lastModifiedDateTime|DateTimeOffset|The date and time when the eBook was last modified. Inherited from [managedEBook](../resources/managedebook.md).|
|privacyInformationUrl|String|The privacy statement Url. Inherited from [managedEBook](../resources/managedebook.md).|
|publishedDateTime|DateTimeOffset|The date and time when the eBook was published. Inherited from [managedEBook](../resources/managedebook.md).|
|publisher|String|Publisher. Inherited from [managedEBook](../resources/managedebook.md).|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|seller|String|Seller.|
|totalLicenseCount|Int32|Total license count.|
|usedLicenseCount|Int32|Used license count.|
|vppOrganizationName|String|The Vpp token's organization name.|
|vppTokenId|Guid|The Vpp token ID.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedEBookAssignment](../resources/managedebookassignment.md) collection|The list of assignments for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|categories|[managedEBookCategory](../resources/managedebookcategory.md) collection|The list of categories for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|deviceStates|[deviceInstallState](../resources/deviceinstallstate.md) collection|The list of installation states for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|
|installSummary|[eBookInstallSummary](../resources/ebookinstallsummary.md)|Mobile App Install Summary. Inherited from [managedEBook](../resources/managedebook.md)|
|userStateSummary|[userInstallStateSummary](../resources/userinstallstatesummary.md) collection|The list of installation states for this eBook. Inherited from [managedEBook](../resources/managedebook.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppEBook",
  "baseType": "microsoft.graph.managedEBook",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppEBook",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "informationUrl": "String",
  "largeCover": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "privacyInformationUrl": "String",
  "publishedDateTime": "String (timestamp)",
  "publisher": "String",
  "appleId": "String",
  "genres": [
    "String"
  ],
  "language": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "seller": "String",
  "totalLicenseCount": "Integer",
  "usedLicenseCount": "Integer",
  "vppOrganizationName": "String",
  "vppTokenId": "Guid"
}
```


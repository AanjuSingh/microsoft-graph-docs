---
title: "drive resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# drive resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [baseItem](../resources/baseitem.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List drives](../api/drive-list.md)|[drive](../resources/drive.md) collection|Get a list of the [drive](../resources/drive.md) objects and their properties.|
|[Create drive](../api/drive-post-drives.md)|[drive](../resources/drive.md)|Create a new [drive](../resources/drive.md) object.|
|[Get drive](../api/drive-get.md)|[drive](../resources/drive.md)|Read the properties and relationships of a [drive](../resources/drive.md) object.|
|[Update drive](../api/drive-update.md)|[drive](../resources/drive.md)|Update the properties of a [drive](../resources/drive.md) object.|
|[Delete drive](../api/drive-delete.md)|None|Deletes a [drive](../resources/drive.md) object.|
|[search](../api/drive-search.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[recent](../api/drive-recent.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[sharedWithMe](../api/drive-sharedwithme.md)|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|[List activities](../api/drive-list-activities.md)|[itemActivityOLD](../resources/itemactivityold.md) collection|Get the itemActivityOLD resources from the activities navigation property.|
|[Create itemActivityOLD](../api/drive-post-activities.md)|[itemActivityOLD](../resources/itemactivityold.md)|Create a new itemActivityOLD object.|
|[List bundles](../api/drive-list-bundles.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItem resources from the bundles navigation property.|
|[Create driveItem](../api/drive-post-bundles.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|
|[List user](../api/drive-list-createdbyuser.md)|[user](../resources/user.md) collection|Get the user resources from the createdByUser navigation property.|
|[Add user](../api/drive-post-createdbyuser.md)|[user](../resources/user.md)|Add createdByUser by posting to the createdByUser collection.|
|[List following](../api/drive-list-following.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItem resources from the following navigation property.|
|[Create driveItem](../api/drive-post-following.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|
|[List items](../api/drive-list-items.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItem resources from the items navigation property.|
|[Create driveItem](../api/drive-post-items.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|
|[List user](../api/drive-list-lastmodifiedbyuser.md)|[user](../resources/user.md) collection|Get the user resources from the lastModifiedByUser navigation property.|
|[Add user](../api/drive-post-lastmodifiedbyuser.md)|[user](../resources/user.md)|Add lastModifiedByUser by posting to the lastModifiedByUser collection.|
|[List list](../api/drive-list-list.md)|[list](../resources/list.md) collection|Get the list resources from the list navigation property.|
|[Create list](../api/drive-post-list.md)|[list](../resources/list.md)|Create a new list object.|
|[List driveItem](../api/drive-list-root.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItem resources from the root navigation property.|
|[Create driveItem](../api/drive-post-root.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|
|[List special](../api/drive-list-special.md)|[driveItem](../resources/driveitem.md) collection|Get the driveItem resources from the special navigation property.|
|[Create driveItem](../api/drive-post-special.md)|[driveItem](../resources/driveitem.md)|Create a new driveItem object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|description|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|driveType|String|**TODO: Add Description**|
|eTag|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|name|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|owner|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|parentReference|[itemReference](../resources/itemreference.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|
|quota|[quota](../resources/quota.md)|**TODO: Add Description**|
|sharePointIds|[sharepointIds](../resources/sharepointids.md)|**TODO: Add Description**|
|system|[systemFacet](../resources/systemfacet.md)|**TODO: Add Description**|
|webUrl|String|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|activities|[itemActivityOLD](../resources/itemactivityold.md) collection|**TODO: Add Description**|
|bundles|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|createdByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|following|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|items|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|
|lastModifiedByUser|[user](../resources/user.md)|**TODO: Add Description** Inherited from [baseItem](../resources/baseitem.md)|
|list|[list](../resources/list.md)|**TODO: Add Description**|
|root|[driveItem](../resources/driveitem.md)|**TODO: Add Description**|
|special|[driveItem](../resources/driveitem.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.drive",
  "baseType": "microsoft.graph.baseItem",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.drive",
  "id": "String (identifier)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "eTag": "String",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "name": "String",
  "parentReference": {
    "@odata.type": "microsoft.graph.itemReference"
  },
  "webUrl": "String",
  "driveType": "String",
  "owner": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "quota": {
    "@odata.type": "microsoft.graph.quota"
  },
  "sharePointIds": {
    "@odata.type": "microsoft.graph.sharepointIds"
  },
  "system": {
    "@odata.type": "microsoft.graph.systemFacet"
  }
}
```


---
title: "unifiedGroupSource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unifiedGroupSource resource type

Namespace: microsoft.graph.ediscovery



**TODO: Add Description**


Inherits from [dataSource](../resources/ediscovery-datasource.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedGroupSources](../api/ediscovery-unifiedgroupsource-list.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) collection|Get a list of the [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) objects and their properties.|
|[Create unifiedGroupSource](../api/ediscovery-unifiedgroupsource-create.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Create a new [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.|
|[Get unifiedGroupSource](../api/ediscovery-unifiedgroupsource-get.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Read the properties and relationships of an [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.|
|[Update unifiedGroupSource](../api/ediscovery-unifiedgroupsource-update.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Update the properties of an [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.|
|[Delete unifiedGroupSource](../api/ediscovery-unifiedgroupsource-delete.md)|None|Deletes an [unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) object.|
|[List group](../api/ediscovery-unifiedgroupsource-list-group.md)|[microsoft.graph.group](../resources/ediscovery-group.md) collection|Get the group resources from the group navigation property.|
|[Add group](../api/ediscovery-unifiedgroupsource-post-group.md)|[microsoft.graph.group](../resources/ediscovery-group.md)|Add group by posting to the group collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description** Inherited from [dataSource](../resources/ediscovery-datasource.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [dataSource](../resources/ediscovery-datasource.md).|
|displayName|String|**TODO: Add Description** Inherited from [dataSource](../resources/ediscovery-datasource.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|
|includedSources|sourceType|**TODO: Add Description**. The possible values are: `mailbox`, `site`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|group|[group](../resources/ediscovery-group.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.unifiedGroupSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.unifiedGroupSource",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "includedSources": "String"
}
```


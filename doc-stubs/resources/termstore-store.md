---
title: "store resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# store resource type

Namespace: microsoft.graph.termStore

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/termstore-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List stores](../api/termstore-store-list.md)|[microsoft.graph.termStore.store](../resources/termstore-store.md) collection|Get a list of the [store](../resources/termstore-store.md) objects and their properties.|
|[Create store](../api/termstore-store-create.md)|[microsoft.graph.termStore.store](../resources/termstore-store.md)|Create a new [store](../resources/termstore-store.md) object.|
|[Get store](../api/termstore-store-get.md)|[microsoft.graph.termStore.store](../resources/termstore-store.md)|Read the properties and relationships of a [store](../resources/termstore-store.md) object.|
|[Update store](../api/termstore-store-update.md)|[microsoft.graph.termStore.store](../resources/termstore-store.md)|Update the properties of a [store](../resources/termstore-store.md) object.|
|[Delete store](../api/termstore-store-delete.md)|None|Deletes a [store](../resources/termstore-store.md) object.|
|[List groups](../api/termstore-store-list-groups.md)|[microsoft.graph.termStore.group](../resources/termstore-group.md) collection|Get the group resources from the groups navigation property.|
|[Create group](../api/termstore-store-post-groups.md)|[microsoft.graph.termStore.group](../resources/termstore-group.md)|Create a new group object.|
|[List sets](../api/termstore-store-list-sets.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md) collection|Get the set resources from the sets navigation property.|
|[Create set](../api/termstore-store-post-sets.md)|[microsoft.graph.termStore.set](../resources/termstore-set.md)|Create a new set object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|defaultLanguageTag|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/termstore-entity.md).|
|languageTags|String collection|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|groups|[microsoft.graph.termStore.group](../resources/termstore-group.md) collection|**TODO: Add Description**|
|sets|[microsoft.graph.termStore.set](../resources/termstore-set.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termStore.store",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termStore.store",
  "id": "String (identifier)",
  "defaultLanguageTag": "String",
  "languageTags": [
    "String"
  ]
}
```


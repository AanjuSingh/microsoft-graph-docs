---
title: "tag resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# tag resource type

Namespace: microsoft.graph.ediscovery



**TODO: Add Description**


Inherits from [entity](../resources/ediscovery-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List tags](../api/ediscovery-tag-list.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection|Get a list of the [tag](../resources/ediscovery-tag.md) objects and their properties.|
|[Create tag](../api/ediscovery-tag-create.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Create a new [tag](../resources/ediscovery-tag.md) object.|
|[Get tag](../api/ediscovery-tag-get.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Read the properties and relationships of a [tag](../resources/ediscovery-tag.md) object.|
|[Update tag](../api/ediscovery-tag-update.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Update the properties of a [tag](../resources/ediscovery-tag.md) object.|
|[Delete tag](../api/ediscovery-tag-delete.md)|None|Deletes a [tag](../resources/ediscovery-tag.md) object.|
|[asHierarchy](../api/ediscovery-tag-ashierarchy.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection|**TODO: Add Description**|
|[List childTags](../api/ediscovery-tag-list-childtags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection|Get the tag resources from the childTags navigation property.|
|[Add tag](../api/ediscovery-tag-post-childtags.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Add childTags by posting to the childTags collection.|
|[List tag](../api/ediscovery-tag-list-parent.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection|Get the tag resources from the parent navigation property.|
|[Add tag](../api/ediscovery-tag-post-parent.md)|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md)|Add parent by posting to the parent collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|childSelectability|childSelectability|**TODO: Add Description**. The possible values are: `One`, `Many`.|
|createdBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|childTags|[microsoft.graph.ediscovery.tag](../resources/ediscovery-tag.md) collection|**TODO: Add Description**|
|parent|[tag](../resources/ediscovery-tag.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.tag",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.tag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "childSelectability": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)"
}
```


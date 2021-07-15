---
title: "cartToClassAssociation resource type"
description: "CartToClassAssociation for associating device carts with classrooms."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# cartToClassAssociation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CartToClassAssociation for associating device carts with classrooms.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List cartToClassAssociations](../api/carttoclassassociation-list.md)|[cartToClassAssociation](../resources/carttoclassassociation.md) collection|Get a list of the [cartToClassAssociation](../resources/carttoclassassociation.md) objects and their properties.|
|[Create cartToClassAssociation](../api/carttoclassassociation-create.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Create a new [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[Get cartToClassAssociation](../api/carttoclassassociation-get.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Read the properties and relationships of a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[Update cartToClassAssociation](../api/carttoclassassociation-update.md)|[cartToClassAssociation](../resources/carttoclassassociation.md)|Update the properties of a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|
|[Delete cartToClassAssociation](../api/carttoclassassociation-delete.md)|None|Deletes a [cartToClassAssociation](../resources/carttoclassassociation.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classroomIds|String collection|Identifiers of classrooms to be associated with device carts.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the CartToClassAssociation.|
|deviceCartIds|String collection|Identifiers of device carts to be associated with classes.|
|displayName|String|Admin provided name of the device configuration.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|version|Int32|Version of the CartToClassAssociation.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cartToClassAssociation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "String (identifier)",
  "classroomIds": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "deviceCartIds": [
    "String"
  ],
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "version": "Integer"
}
```


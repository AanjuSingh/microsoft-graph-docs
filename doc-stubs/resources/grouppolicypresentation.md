---
title: "groupPolicyPresentation resource type"
description: "The base entity for the display presentation of any of the additional options in a group policy definition."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# groupPolicyPresentation resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The base entity for the display presentation of any of the additional options in a group policy definition.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List groupPolicyPresentations](../api/grouppolicypresentation-list.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md) collection|Get a list of the [groupPolicyPresentation](../resources/grouppolicypresentation.md) objects and their properties.|
|[Create groupPolicyPresentation](../api/grouppolicypresentation-create.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Create a new [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Get groupPolicyPresentation](../api/grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Read the properties and relationships of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Update groupPolicyPresentation](../api/grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/grouppolicypresentation.md)|Update the properties of a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[Delete groupPolicyPresentation](../api/grouppolicypresentation-delete.md)|None|Deletes a [groupPolicyPresentation](../resources/grouppolicypresentation.md) object.|
|[List groupPolicyDefinition](../api/grouppolicypresentation-list-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md) collection|Get the groupPolicyDefinition resources from the definition navigation property.|
|[Add groupPolicyDefinition](../api/grouppolicypresentation-post-definition.md)|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|Add definition by posting to the definition collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|label|String|Localized text label for any presentation entity. The default value is empty.|
|lastModifiedDateTime|DateTimeOffset|The date and time the entity was last modified.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/grouppolicydefinition.md)|The group policy definition associated with the presentation.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "id": "String (identifier)",
  "label": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```


---
title: "educationPointsOutcome resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationPointsOutcome resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [educationOutcome](../resources/educationoutcome.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List educationPointsOutcomes](../api/educationpointsoutcome-list.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md) collection|Get a list of the [educationPointsOutcome](../resources/educationpointsoutcome.md) objects and their properties.|
|[Create educationPointsOutcome](../api/educationpointsoutcome-create.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md)|Create a new [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Get educationPointsOutcome](../api/educationpointsoutcome-get.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md)|Read the properties and relationships of an [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Update educationPointsOutcome](../api/educationpointsoutcome-update.md)|[educationPointsOutcome](../resources/educationpointsoutcome.md)|Update the properties of an [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|
|[Delete educationPointsOutcome](../api/educationpointsoutcome-delete.md)|None|Deletes an [educationPointsOutcome](../resources/educationpointsoutcome.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [educationOutcome](../resources/educationoutcome.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [educationOutcome](../resources/educationoutcome.md).|
|points|[educationAssignmentPointsGrade](../resources/educationassignmentpointsgrade.md)|**TODO: Add Description**|
|publishedPoints|[educationAssignmentPointsGrade](../resources/educationassignmentpointsgrade.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationPointsOutcome",
  "baseType": "microsoft.graph.educationOutcome",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationPointsOutcome",
  "id": "String (identifier)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "points": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
  },
  "publishedPoints": {
    "@odata.type": "microsoft.graph.educationAssignmentPointsGrade"
  }
}
```


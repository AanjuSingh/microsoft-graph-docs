---
title: "termsAndConditionsGroupAssignment resource type"
description: "A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (TandC) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# termsAndConditionsGroupAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A termsAndConditionsGroupAssignment entity represents the assignment of a given Terms and Conditions (TandC) policy to a given group. Users in the group will be required to accept the terms in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List termsAndConditionsGroupAssignments](../api/termsandconditionsgroupassignment-list.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|Get a list of the [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) objects and their properties.|
|[Create termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-create.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Create a new [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Get termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Read the properties and relationships of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Update termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Update the properties of a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[Delete termsAndConditionsGroupAssignment](../api/termsandconditionsgroupassignment-delete.md)|None|Deletes a [termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) object.|
|[List termsAndConditions](../api/termsandconditionsgroupassignment-list-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get the termsAndConditions resources from the termsAndConditions navigation property.|
|[Add termsAndConditions](../api/termsandconditionsgroupassignment-post-termsandconditions.md)|[termsAndConditions](../resources/termsandconditions.md)|Add termsAndConditions by posting to the termsAndConditions collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|targetGroupId|String|Unique identifier of a group that the TandC policy is assigned to.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/termsandconditions.md)|Navigation link to the terms and conditions that are assigned.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```


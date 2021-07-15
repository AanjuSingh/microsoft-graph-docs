---
title: "termsAndConditions resource type"
description: "A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (TandC) policy. TandC policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance. They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# termsAndConditions resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A termsAndConditions entity represents the metadata and contents of a given Terms and Conditions (TandC) policy. TandC policies’ contents are presented to users upon their first attempt to enroll into Intune and subsequently upon edits where an administrator has required re-acceptance. They enable administrators to communicate the provisions to which a user must agree in order to have devices enrolled into Intune.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List termsAndConditions](../api/termsandconditions-list.md)|[termsAndConditions](../resources/termsandconditions.md) collection|Get a list of the [termsAndConditions](../resources/termsandconditions.md) objects and their properties.|
|[Create termsAndConditions](../api/termsandconditions-create.md)|[termsAndConditions](../resources/termsandconditions.md)|Create a new [termsAndConditions](../resources/termsandconditions.md) object.|
|[Get termsAndConditions](../api/termsandconditions-get.md)|[termsAndConditions](../resources/termsandconditions.md)|Read the properties and relationships of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[Update termsAndConditions](../api/termsandconditions-update.md)|[termsAndConditions](../resources/termsandconditions.md)|Update the properties of a [termsAndConditions](../resources/termsandconditions.md) object.|
|[Delete termsAndConditions](../api/termsandconditions-delete.md)|None|Deletes a [termsAndConditions](../resources/termsandconditions.md) object.|
|[List acceptanceStatuses](../api/termsandconditions-list-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|Get the termsAndConditionsAcceptanceStatus resources from the acceptanceStatuses navigation property.|
|[Create termsAndConditionsAcceptanceStatus](../api/termsandconditions-post-acceptancestatuses.md)|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md)|Create a new termsAndConditionsAcceptanceStatus object.|
|[List assignments](../api/termsandconditions-list-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|Get the termsAndConditionsAssignment resources from the assignments navigation property.|
|[Create termsAndConditionsAssignment](../api/termsandconditions-post-assignments.md)|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md)|Create a new termsAndConditionsAssignment object.|
|[List groupAssignments](../api/termsandconditions-list-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|Get the termsAndConditionsGroupAssignment resources from the groupAssignments navigation property.|
|[Create termsAndConditionsGroupAssignment](../api/termsandconditions-post-groupassignments.md)|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md)|Create a new termsAndConditionsGroupAssignment object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptanceStatement|String|Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the TandC policy. This is shown to the user on prompts to accept the TandC policy.|
|bodyText|String|Administrator-supplied body text of the terms and conditions, typically the terms themselves. This is shown to the user on prompts to accept the TandC policy.|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Administrator-supplied description of the TandC policy.|
|displayName|String|Administrator-supplied name for the TandC policy. |
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|modifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|title|String|Administrator-supplied title of the terms and conditions. This is shown to the user on prompts to accept the TandC policy.|
|version|Int32|Integer indicating the current version of the terms. Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified TandC policy.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|acceptanceStatuses|[termsAndConditionsAcceptanceStatus](../resources/termsandconditionsacceptancestatus.md) collection|The list of acceptance statuses for this TandC policy.|
|assignments|[termsAndConditionsAssignment](../resources/termsandconditionsassignment.md) collection|The list of assignments for this TandC policy.|
|groupAssignments|[termsAndConditionsGroupAssignment](../resources/termsandconditionsgroupassignment.md) collection|The list of group assignments for this TandC policy.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditions",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "String (identifier)",
  "acceptanceStatement": "String",
  "bodyText": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "title": "String",
  "version": "Integer"
}
```


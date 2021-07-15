---
title: "educationClass resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# educationClass resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List educationClasses](../api/educationclass-list.md)|[educationClass](../resources/educationclass.md) collection|Get a list of the [educationClass](../resources/educationclass.md) objects and their properties.|
|[Create educationClass](../api/educationclass-create.md)|[educationClass](../resources/educationclass.md)|Create a new [educationClass](../resources/educationclass.md) object.|
|[Get educationClass](../api/educationclass-get.md)|[educationClass](../resources/educationclass.md)|Read the properties and relationships of an [educationClass](../resources/educationclass.md) object.|
|[Update educationClass](../api/educationclass-update.md)|[educationClass](../resources/educationclass.md)|Update the properties of an [educationClass](../resources/educationclass.md) object.|
|[Delete educationClass](../api/educationclass-delete.md)|None|Deletes an [educationClass](../resources/educationclass.md) object.|
|[delta](../api/educationclass-delta.md)|[educationClass](../resources/educationclass.md) collection|**TODO: Add Description**|
|[List assignmentCategories](../api/educationclass-list-assignmentcategories.md)|[educationCategory](../resources/educationcategory.md) collection|Get the educationCategory resources from the assignmentCategories navigation property.|
|[Create educationCategory](../api/educationclass-post-assignmentcategories.md)|[educationCategory](../resources/educationcategory.md)|Create a new educationCategory object.|
|[List educationAssignmentDefaults](../api/educationclass-list-assignmentdefaults.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md) collection|Get the educationAssignmentDefaults resources from the assignmentDefaults navigation property.|
|[Create educationAssignmentDefaults](../api/educationclass-post-assignmentdefaults.md)|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|Create a new educationAssignmentDefaults object.|
|[List assignments](../api/educationclass-list-assignments.md)|[educationAssignment](../resources/educationassignment.md) collection|Get the educationAssignment resources from the assignments navigation property.|
|[Create educationAssignment](../api/educationclass-post-assignments.md)|[educationAssignment](../resources/educationassignment.md)|Create a new educationAssignment object.|
|[List educationAssignmentSettings](../api/educationclass-list-assignmentsettings.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md) collection|Get the educationAssignmentSettings resources from the assignmentSettings navigation property.|
|[Create educationAssignmentSettings](../api/educationclass-post-assignmentsettings.md)|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|Create a new educationAssignmentSettings object.|
|[List group](../api/educationclass-list-group.md)|[group](../resources/group.md) collection|Get the group resources from the group navigation property.|
|[Add group](../api/educationclass-post-group.md)|[group](../resources/group.md)|Add group by posting to the group collection.|
|[List members](../api/educationclass-list-members.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUser resources from the members navigation property.|
|[Add educationUser](../api/educationclass-post-members.md)|[educationUser](../resources/educationuser.md)|Add members by posting to the members collection.|
|[List schools](../api/educationclass-list-schools.md)|[educationSchool](../resources/educationschool.md) collection|Get the educationSchool resources from the schools navigation property.|
|[Add educationSchool](../api/educationclass-post-schools.md)|[educationSchool](../resources/educationschool.md)|Add schools by posting to the schools collection.|
|[List teachers](../api/educationclass-list-teachers.md)|[educationUser](../resources/educationuser.md) collection|Get the educationUser resources from the teachers navigation property.|
|[Add educationUser](../api/educationclass-post-teachers.md)|[educationUser](../resources/educationuser.md)|Add teachers by posting to the teachers collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|classCode|String|**TODO: Add Description**|
|course|[educationCourse](../resources/educationcourse.md)|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|externalId|String|**TODO: Add Description**|
|externalName|String|**TODO: Add Description**|
|externalSource|educationExternalSource|**TODO: Add Description**. Possible values are: `sis`, `manual`, `unknownFutureValue`, `lms`.|
|externalSourceDetail|String|**TODO: Add Description**|
|grade|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|mailNickname|String|**TODO: Add Description**|
|term|[educationTerm](../resources/educationterm.md)|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignmentCategories|[educationCategory](../resources/educationcategory.md) collection|**TODO: Add Description**|
|assignmentDefaults|[educationAssignmentDefaults](../resources/educationassignmentdefaults.md)|**TODO: Add Description**|
|assignments|[educationAssignment](../resources/educationassignment.md) collection|**TODO: Add Description**|
|assignmentSettings|[educationAssignmentSettings](../resources/educationassignmentsettings.md)|**TODO: Add Description**|
|group|[group](../resources/group.md)|**TODO: Add Description**|
|members|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|
|schools|[educationSchool](../resources/educationschool.md) collection|**TODO: Add Description**|
|teachers|[educationUser](../resources/educationuser.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationClass",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.educationClass",
  "id": "String (identifier)",
  "classCode": "String",
  "course": {
    "@odata.type": "microsoft.graph.educationCourse"
  },
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "String",
  "externalSourceDetail": "String",
  "grade": "String",
  "mailNickname": "String",
  "term": {
    "@odata.type": "microsoft.graph.educationTerm"
  }
}
```


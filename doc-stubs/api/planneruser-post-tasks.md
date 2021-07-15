---
title: "Add plannerTask"
description: "Add tasks by posting to the tasks collection."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Add plannerTask
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Add tasks by posting to the tasks collection.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/planner/tasks/$ref
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerTask](../resources/plannertask.md) object.

The following table shows the properties that are required when you create the [plannerTask](../resources/plannertask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activeChecklistItemCount|Int32|**TODO: Add Description**|
|appliedCategories|[plannerAppliedCategories](../resources/plannerappliedcategories.md)|**TODO: Add Description**|
|assigneePriority|String|**TODO: Add Description**|
|assignments|[plannerAssignments](../resources/plannerassignments.md)|**TODO: Add Description**|
|bucketId|String|**TODO: Add Description**|
|checklistItemCount|Int32|**TODO: Add Description**|
|completedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|completedDateTime|DateTimeOffset|**TODO: Add Description**|
|conversationThreadId|String|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|creationSource|[plannerTaskCreation](../resources/plannertaskcreation.md)|**TODO: Add Description**|
|dueDateTime|DateTimeOffset|**TODO: Add Description**|
|hasDescription|Boolean|**TODO: Add Description**|
|orderHint|String|**TODO: Add Description**|
|percentComplete|Int32|**TODO: Add Description**|
|planId|String|**TODO: Add Description**|
|previewType|plannerPreviewType|**TODO: Add Description**. Possible values are: `automatic`, `noPreview`, `checklist`, `description`, `reference`.|
|priority|Int32|**TODO: Add Description**|
|referenceCount|Int32|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|title|String|**TODO: Add Description**|



## Response

If successful, this method returns a `204 No Content` response code and a [plannerTask](../resources/plannertask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannertask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/planner/tasks/$ref
Content-Type: application/json
Content-length: 991

{
  "@odata.type": "#microsoft.graph.plannerTask",
  "activeChecklistItemCount": "Integer",
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assigneePriority": "String",
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "bucketId": "String",
  "checklistItemCount": "Integer",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "creationSource": {
    "@odata.type": "microsoft.graph.plannerTaskCreation"
  },
  "dueDateTime": "String (timestamp)",
  "hasDescription": "Boolean",
  "orderHint": "String",
  "percentComplete": "Integer",
  "planId": "String",
  "previewType": "String",
  "priority": "Integer",
  "referenceCount": "Integer",
  "startDateTime": "String (timestamp)",
  "title": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerTask"
}
-->
``` http
HTTP/1.1 204 No Content
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerTask",
  "id": "bd7a91e1-91e1-bd7a-e191-7abde1917abd",
  "activeChecklistItemCount": "Integer",
  "appliedCategories": {
    "@odata.type": "microsoft.graph.plannerAppliedCategories"
  },
  "assigneePriority": "String",
  "assignments": {
    "@odata.type": "microsoft.graph.plannerAssignments"
  },
  "bucketId": "String",
  "checklistItemCount": "Integer",
  "completedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "completedDateTime": "String (timestamp)",
  "conversationThreadId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "creationSource": {
    "@odata.type": "microsoft.graph.plannerTaskCreation"
  },
  "dueDateTime": "String (timestamp)",
  "hasDescription": "Boolean",
  "orderHint": "String",
  "percentComplete": "Integer",
  "planId": "String",
  "previewType": "String",
  "priority": "Integer",
  "referenceCount": "Integer",
  "startDateTime": "String (timestamp)",
  "title": "String"
}
```


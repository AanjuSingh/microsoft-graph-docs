---
title: "Create outlookTask"
description: "Create a new outlookTask object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create outlookTask
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new outlookTask object.

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
POST /users/{usersId}/outlook/taskFolders/{outlookTaskFolderId}/tasks
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [outlookTask](../resources/outlooktask.md) object.

The following table shows the properties that are required when you create the [outlookTask](../resources/outlooktask.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|categories|String collection|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|changeKey|String|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [outlookItem](../resources/outlookitem.md)|
|assignedTo|String|**TODO: Add Description**|
|body|[itemBody](../resources/itembody.md)|**TODO: Add Description**|
|completedDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|dueDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|hasAttachments|Boolean|**TODO: Add Description**|
|importance|importance|**TODO: Add Description**. Possible values are: `low`, `normal`, `high`.|
|isReminderOn|Boolean|**TODO: Add Description**|
|owner|String|**TODO: Add Description**|
|parentFolderId|String|**TODO: Add Description**|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|**TODO: Add Description**|
|reminderDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|sensitivity|sensitivity|**TODO: Add Description**. Possible values are: `normal`, `personal`, `private`, `confidential`.|
|startDateTime|[dateTimeTimeZone](../resources/datetimetimezone.md)|**TODO: Add Description**|
|status|taskStatus|**TODO: Add Description**. Possible values are: `notStarted`, `inProgress`, `completed`, `waitingOnOthers`, `deferred`.|
|subject|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [outlookTask](../resources/outlooktask.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_outlooktask_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/outlook/taskFolders/{outlookTaskFolderId}/tasks
Content-Type: application/json
Content-length: 848

{
  "@odata.type": "#microsoft.graph.outlookTask",
  "categories": [
    "String"
  ],
  "changeKey": "String",
  "assignedTo": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "hasAttachments": "Boolean",
  "importance": "String",
  "isReminderOn": "Boolean",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "sensitivity": "String",
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "subject": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTask"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.outlookTask",
  "id": "5f0e17fa-17fa-5f0e-fa17-0e5ffa170e5f",
  "categories": [
    "String"
  ],
  "changeKey": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "assignedTo": "String",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "completedDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "dueDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "hasAttachments": "Boolean",
  "importance": "String",
  "isReminderOn": "Boolean",
  "owner": "String",
  "parentFolderId": "String",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "sensitivity": "String",
  "startDateTime": {
    "@odata.type": "microsoft.graph.dateTimeTimeZone"
  },
  "status": "String",
  "subject": "String"
}
```


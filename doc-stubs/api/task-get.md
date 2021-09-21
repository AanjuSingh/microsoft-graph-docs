---
title: "Get task"
description: "Read the properties and relationships of a task object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get task
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [task](../resources/task.md) object.

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
GET /user/tasks/alltasks/{taskId}
GET /user/tasks/lists/{wellKnownTaskListId}/tasks/{taskId}
GET /user/tasks/lists/{wellKnownTaskListId}/tasks/{taskId}/parentList/tasks/{taskId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [task](../resources/task.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_task"
}
-->
``` http
GET https://graph.microsoft.com/beta/user/tasks/alltasks/{taskId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.task"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.task",
    "body": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedDateTime": "String (timestamp)",
    "bodyLastModifiedDateTime": "String (timestamp)",
    "completedDateTime": "String (timestamp)",
    "dueDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "startDateTime": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "importance": "String",
    "recurrence": {
      "@odata.type": "microsoft.graph.patternedRecurrence"
    },
    "displayName": "String",
    "status": "String",
    "personalProperties": {
      "@odata.type": "microsoft.graph.personalTaskProperties"
    },
    "id": "f3371abc-1abc-f337-bc1a-37f3bc1a37f3"
  }
}
```


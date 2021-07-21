---
title: "Get unifiedRoleAssignmentSchedule"
description: "Read the properties and relationships of an unifiedRoleAssignmentSchedule object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get unifiedRoleAssignmentSchedule
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object.

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
GET /roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentScheduleId}
GET /roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestId}/targetSchedule
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

If successful, this method returns a `200 OK` response code and an [unifiedRoleAssignmentSchedule](../resources/unifiedroleassignmentschedule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_unifiedroleassignmentschedule"
}
-->
``` http
GET https://graph.microsoft.com/beta/roleManagement/directory/roleAssignmentSchedules/{unifiedRoleAssignmentScheduleId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentSchedule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.unifiedRoleAssignmentSchedule",
    "id": "2cbc6f14-6f14-2cbc-146f-bc2c146fbc2c",
    "appScopeId": "String",
    "createdDateTime": "String (timestamp)",
    "createdUsing": "String",
    "directoryScopeId": "String",
    "modifiedDateTime": "String (timestamp)",
    "principalId": "String",
    "roleDefinitionId": "String",
    "status": "String",
    "assignmentType": "String",
    "memberType": "String",
    "scheduleInfo": {
      "@odata.type": "microsoft.graph.requestSchedule"
    }
  }
}
```


---
title: "Create educationAssignmentSettings"
description: "Create a new educationAssignmentSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create educationAssignmentSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new educationAssignmentSettings object.

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
POST /education/classes/{educationClassId}/assignmentSettings
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.

The following table shows the properties that are required when you create the [educationAssignmentSettings](../resources/educationassignmentsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|submissionAnimationDisabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_educationassignmentsettings_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignmentSettings
Content-Type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.educationAssignmentSettings",
  "submissionAnimationDisabled": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentSettings"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationAssignmentSettings",
  "id": "16d92091-2091-16d9-9120-d9169120d916",
  "submissionAnimationDisabled": "Boolean"
}
```


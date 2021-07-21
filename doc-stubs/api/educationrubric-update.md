---
title: "Update educationRubric"
description: "Update the properties of an educationRubric object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update educationRubric
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [educationRubric](../resources/educationrubric.md) object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
PATCH /education/classes/{educationClassId}/members/{educationUserId}/rubrics/{educationRubricId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationRubric](../resources/educationrubric.md) object.

The following table shows the properties that are required when you update the [educationRubric](../resources/educationrubric.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|description|[educationItemBody](../resources/educationitembody.md)|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|grading|[educationAssignmentGradeType](../resources/educationassignmentgradetype.md)|**TODO: Add Description**|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|levels|[rubricLevel](../resources/rubriclevel.md) collection|**TODO: Add Description**|
|qualities|[rubricQuality](../resources/rubricquality.md) collection|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [educationRubric](../resources/educationrubric.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_educationrubric"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/rubric
Content-Type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.educationRubric",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody"
  },
  "displayName": "String",
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
  "levels": [
    {
      "@odata.type": "microsoft.graph.rubricLevel"
    }
  ],
  "qualities": [
    {
      "@odata.type": "microsoft.graph.rubricQuality"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.educationRubric",
  "id": "5801befb-befb-5801-fbbe-0158fbbe0158",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "description": {
    "@odata.type": "microsoft.graph.educationItemBody"
  },
  "displayName": "String",
  "grading": {
    "@odata.type": "microsoft.graph.educationAssignmentGradeType"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "levels": [
    {
      "@odata.type": "microsoft.graph.rubricLevel"
    }
  ],
  "qualities": [
    {
      "@odata.type": "microsoft.graph.rubricQuality"
    }
  ]
}
```


---
title: "Update educationAssignmentResource"
description: "Update the properties of an educationAssignmentResource object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update educationAssignmentResource
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [educationAssignmentResource](../resources/educationassignmentresource.md) object.

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
PATCH /education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [educationAssignmentResource](../resources/educationassignmentresource.md) object.

The following table shows the properties that are required when you update the [educationAssignmentResource](../resources/educationassignmentresource.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|distributeForStudentWork|Boolean|**TODO: Add Description**|
|resource|[educationResource](../resources/educationresource.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_educationassignmentresource"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/resources/{educationAssignmentResourceId}
Content-Type: application/json
Content-length: 190

{
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "distributeForStudentWork": "Boolean",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  }
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
  "@odata.type": "#microsoft.graph.educationAssignmentResource",
  "id": "76f38079-8079-76f3-7980-f3767980f376",
  "distributeForStudentWork": "Boolean",
  "resource": {
    "@odata.type": "microsoft.graph.educationResource"
  }
}
```


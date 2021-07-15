---
title: "educationSubmission: submit"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# educationSubmission: submit
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
POST /education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/submit
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this action returns a `200 OK` response code and a [educationSubmission](../resources/educationsubmission.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "educationsubmission_submit"
}
-->
``` http
POST https://graph.microsoft.com/beta/education/classes/{educationClassId}/assignments/{educationAssignmentId}/submissions/{educationSubmissionId}/submit
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSubmission",
    "id": "String (identifier)",
    "recipient": {
      "@odata.type": "microsoft.graph.educationSubmissionRecipient"
    },
    "resourcesFolderUrl": "String",
    "returnedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "returnedDateTime": "String (timestamp)",
    "status": "String",
    "submittedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "submittedDateTime": "String (timestamp)",
    "unsubmittedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "unsubmittedDateTime": "String (timestamp)"
  }
}
```


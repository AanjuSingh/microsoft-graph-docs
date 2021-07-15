---
title: "List accessReviewScheduleDefinition"
description: "Get the accessReviewScheduleDefinition resources from the definition navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List accessReviewScheduleDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the accessReviewScheduleDefinition resources from the definition navigation property.

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
GET /users/{usersId}/pendingAccessReviewInstances/{accessReviewInstanceId}/definition
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

If successful, this method returns a `200 OK` response code and a collection of [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_accessreviewscheduledefinition"
}
-->
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/pendingAccessReviewInstances/{accessReviewInstanceId}/definition
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewScheduleDefinition)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessReviewScheduleDefinition",
      "id": "92d756ba-56ba-92d7-ba56-d792ba56d792",
      "additionalNotificationRecipients": [
        {
          "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem"
        }
      ],
      "backupReviewers": [
        {
          "@odata.type": "microsoft.graph.accessReviewReviewerScope"
        }
      ],
      "createdBy": {
        "@odata.type": "microsoft.graph.userIdentity"
      },
      "createdDateTime": "String (timestamp)",
      "descriptionForAdmins": "String",
      "descriptionForReviewers": "String",
      "displayName": "String",
      "fallbackReviewers": [
        {
          "@odata.type": "microsoft.graph.accessReviewReviewerScope"
        }
      ],
      "instanceEnumerationScope": {
        "@odata.type": "microsoft.graph.accessReviewScope"
      },
      "lastModifiedDateTime": "String (timestamp)",
      "reviewers": [
        {
          "@odata.type": "microsoft.graph.accessReviewReviewerScope"
        }
      ],
      "scope": {
        "@odata.type": "microsoft.graph.accessReviewScope"
      },
      "settings": {
        "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
      },
      "status": "String"
    }
  ]
}
```


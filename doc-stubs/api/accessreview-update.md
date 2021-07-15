---
title: "Update accessReview"
description: "Update the properties of an accessReview object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessReview
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [accessReview](../resources/accessreview.md) object.

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
PATCH /accessReviews/{accessReviewsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessReview](../resources/accessreview.md) object.

The following table shows the properties that are required when you update the [accessReview](../resources/accessreview.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|businessFlowTemplateId|String|**TODO: Add Description**|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|endDateTime|DateTimeOffset|**TODO: Add Description**|
|reviewedEntity|[identity](../resources/identity.md)|**TODO: Add Description**|
|reviewerType|String|**TODO: Add Description**|
|settings|[accessReviewSettings](../resources/accessreviewsettings.md)|**TODO: Add Description**|
|startDateTime|DateTimeOffset|**TODO: Add Description**|
|status|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessReview](../resources/accessreview.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accessreview"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/accessReviews/{accessReviewsId}
Content-Type: application/json
Content-length: 516

{
  "@odata.type": "#microsoft.graph.accessReview",
  "businessFlowTemplateId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "description": "String",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "reviewedEntity": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewerType": "String",
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewSettings"
  },
  "startDateTime": "String (timestamp)",
  "status": "String"
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
  "@odata.type": "#microsoft.graph.accessReview",
  "id": "1bc1239b-239b-1bc1-9b23-c11b9b23c11b",
  "businessFlowTemplateId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "description": "String",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "reviewedEntity": {
    "@odata.type": "microsoft.graph.identity"
  },
  "reviewerType": "String",
  "settings": {
    "@odata.type": "microsoft.graph.accessReviewSettings"
  },
  "startDateTime": "String (timestamp)",
  "status": "String"
}
```


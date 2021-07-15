---
title: "Create plannerPlanDetails"
description: "Create a new plannerPlanDetails object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create plannerPlanDetails
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new plannerPlanDetails object.

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
POST /users/{usersId}/planner/favoritePlans/{plannerPlanId}/details
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [plannerPlanDetails](../resources/plannerplandetails.md) object.

The following table shows the properties that are required when you create the [plannerPlanDetails](../resources/plannerplandetails.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|categoryDescriptions|[plannerCategoryDescriptions](../resources/plannercategorydescriptions.md)|**TODO: Add Description**|
|contextDetails|[plannerPlanContextDetailsCollection](../resources/plannerplancontextdetailscollection.md)|**TODO: Add Description**|
|sharedWith|[plannerUserIds](../resources/planneruserids.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [plannerPlanDetails](../resources/plannerplandetails.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_plannerplandetails_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/planner/favoritePlans/{plannerPlanId}/details
Content-Type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  },
  "contextDetails": {
    "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
  },
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerPlanDetails"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.plannerPlanDetails",
  "id": "50b5443b-443b-50b5-3b44-b5503b44b550",
  "categoryDescriptions": {
    "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
  },
  "contextDetails": {
    "@odata.type": "microsoft.graph.plannerPlanContextDetailsCollection"
  },
  "sharedWith": {
    "@odata.type": "microsoft.graph.plannerUserIds"
  }
}
```


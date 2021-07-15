---
title: "Update accessReviewHistoryDefinition"
description: "Update the properties of an accessReviewHistoryDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update accessReviewHistoryDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.

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
PATCH /identityGovernance/accessReviews/historyDefinitions/{accessReviewHistoryDefinitionId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object.

The following table shows the properties that are required when you update the [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[userIdentity](../resources/useridentity.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|decisions|accessReviewHistoryDecisionFilter collection|**TODO: Add Description**. Possible values are: `approve`, `deny`, `notReviewed`, `dontKnow`, `notNotified`, `unknownFutureValue`.|
|displayName|String|**TODO: Add Description**|
|downloadUri|String|**TODO: Add Description**|
|fulfilledDateTime|DateTimeOffset|**TODO: Add Description**|
|reviewHistoryPeriodEndDateTime|DateTimeOffset|**TODO: Add Description**|
|reviewHistoryPeriodStartDateTime|DateTimeOffset|**TODO: Add Description**|
|scopes|[accessReviewScope](../resources/accessreviewscope.md) collection|**TODO: Add Description**|
|status|accessReviewHistoryStatus|**TODO: Add Description**. Possible values are: `done`, `inprogress`, `error`, `requested`, `unknownFutureValue`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [accessReviewHistoryDefinition](../resources/accessreviewhistorydefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_accessreviewhistorydefinition"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/historyDefinitions/{accessReviewHistoryDefinitionId}
Content-Type: application/json
Content-length: 522

{
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "decisions": [
    "String"
  ],
  "displayName": "String",
  "downloadUri": "String",
  "fulfilledDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "scopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
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
  "@odata.type": "#microsoft.graph.accessReviewHistoryDefinition",
  "id": "0a52d0dc-d0dc-0a52-dcd0-520adcd0520a",
  "createdBy": {
    "@odata.type": "microsoft.graph.userIdentity"
  },
  "createdDateTime": "String (timestamp)",
  "decisions": [
    "String"
  ],
  "displayName": "String",
  "downloadUri": "String",
  "fulfilledDateTime": "String (timestamp)",
  "reviewHistoryPeriodEndDateTime": "String (timestamp)",
  "reviewHistoryPeriodStartDateTime": "String (timestamp)",
  "scopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "status": "String"
}
```


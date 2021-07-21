---
title: "Create riskyUserHistoryItem"
description: "Create a new riskyUserHistoryItem object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create riskyUserHistoryItem
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

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
POST /riskyUsers/{riskyUsersId}/history
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.

The following table shows the properties that are required when you create the [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|isDeleted|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|isProcessing|Boolean|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|riskDetail|riskDetail|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.|
|riskLastUpdatedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|riskLevel|riskLevel|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`.|
|riskState|riskState|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md). Possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`.|
|userDisplayName|String|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|userPrincipalName|String|**TODO: Add Description** Inherited from [riskyUser](../resources/riskyuser.md)|
|activity|[riskUserActivity](../resources/riskuseractivity.md)|**TODO: Add Description**|
|initiatedBy|String|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_riskyuserhistoryitem_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/riskyUsers/{riskyUsersId}/history
Content-Type: application/json
Content-length: 445

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskDetail": "String",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  },
  "initiatedBy": "String",
  "userId": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
  "id": "b712ea89-ea89-b712-89ea-12b789ea12b7",
  "isDeleted": "Boolean",
  "isProcessing": "Boolean",
  "riskDetail": "String",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "riskLevel": "String",
  "riskState": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "activity": {
    "@odata.type": "microsoft.graph.riskUserActivity"
  },
  "initiatedBy": "String",
  "userId": "String"
}
```


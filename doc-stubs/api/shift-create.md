---
title: "Create shift"
description: "Create a new shift object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create shift
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [shift](../resources/shift.md) object.

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
POST /team/schedule/shifts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [shift](../resources/shift.md) object.

The following table shows the properties that are required when you create the [shift](../resources/shift.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|createdBy|[Microsoft.Teams.Shifts.identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[Microsoft.Teams.Shifts.identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|sharedShift|[Microsoft.Teams.Shifts.shiftItem](../resources/shiftitem.md)|**TODO: Add Description**|
|draftShift|[Microsoft.Teams.Shifts.shiftItem](../resources/shiftitem.md)|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|
|schedulingGroupId|String|**TODO: Add Description**|
|isStagedForDeletion|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_shift_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/team/schedule/shifts
Content-Type: application/json
Content-length: 369

{
  "@odata.type": "#Microsoft.Teams.Shifts.shift",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "String",
  "schedulingGroupId": "String",
  "isStagedForDeletion": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.Teams.Shifts.shift"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.Teams.Shifts.shift",
  "id": "fe55afb0-afb0-fe55-b0af-55feb0af55fe",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "sharedShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "draftShift": {
    "@odata.type": "microsoft.graph.shiftItem"
  },
  "userId": "String",
  "schedulingGroupId": "String",
  "isStagedForDeletion": "Boolean"
}
```


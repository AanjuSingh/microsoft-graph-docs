---
title: "Update timeOff"
description: "Update the properties of a timeOff object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update timeOff
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [timeOff](../resources/timeoff.md) object.

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
PATCH /teams/{teamsId}/schedule/timesOff/{timeOffId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [timeOff](../resources/timeoff.md) object.

The following table shows the properties that are required when you update the [timeOff](../resources/timeoff.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [changeTrackedEntity](../resources/changetrackedentity.md)|
|draftTimeOff|[timeOffItem](../resources/timeoffitem.md)|**TODO: Add Description**|
|isStagedForDeletion|Boolean|**TODO: Add Description**|
|sharedTimeOff|[timeOffItem](../resources/timeoffitem.md)|**TODO: Add Description**|
|userId|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [timeOff](../resources/timeoff.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_timeoff"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teams/{teamsId}/schedule/timesOff/{timeOffId}
Content-Type: application/json
Content-length: 338

{
  "@odata.type": "#microsoft.graph.timeOff",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "isStagedForDeletion": "Boolean",
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "String"
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
  "@odata.type": "#microsoft.graph.timeOff",
  "id": "d9a7788a-788a-d9a7-8a78-a7d98a78a7d9",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "draftTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "isStagedForDeletion": "Boolean",
  "sharedTimeOff": {
    "@odata.type": "microsoft.graph.timeOffItem"
  },
  "userId": "String"
}
```


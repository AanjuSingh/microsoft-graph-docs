---
title: "timeCard: clockIn"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# timeCard: clockIn
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
POST /teams/{teamsId}/schedule/timeCards/clockIn
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|atApprovedLocation|Boolean|**TODO: Add Description**|
|onBehalfOfUserId|String|**TODO: Add Description**|
|notes|[itemBody](../resources/itembody.md)|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [timeCard](../resources/timecard.md) in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "timecard_clockin"
}
-->
``` http
POST https://graph.microsoft.com/beta/teams/{teamsId}/schedule/timeCards/clockIn
Content-Type: application/json
Content-length: 139

{
  "atApprovedLocation": "Boolean",
  "onBehalfOfUserId": "String",
  "notes": {
    "@odata.type": "microsoft.graph.itemBody"
  }
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeCard"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.timeCard",
    "id": "String (identifier)",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "breaks": [
      {
        "@odata.type": "microsoft.graph.timeCardBreak"
      }
    ],
    "clockInEvent": {
      "@odata.type": "microsoft.graph.timeCardEvent"
    },
    "clockOutEvent": {
      "@odata.type": "microsoft.graph.timeCardEvent"
    },
    "confirmedBy": "String",
    "notes": {
      "@odata.type": "microsoft.graph.itemBody"
    },
    "originalEntry": {
      "@odata.type": "microsoft.graph.timeCardEntry"
    },
    "state": "String",
    "userId": "String"
  }
}
```


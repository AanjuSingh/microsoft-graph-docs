---
title: "Update teamsUserActivityCounts"
description: "Update the properties of a teamsUserActivityCounts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update teamsUserActivityCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object.

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
PATCH /teamsUserActivityCounts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object.

The following table shows the properties that are required when you update the [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|calls|Int64|**TODO: Add Description**|
|meetings|Int64|**TODO: Add Description**|
|privateChatMessages|Int64|**TODO: Add Description**|
|reportDate|Date|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|teamChatMessages|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [teamsUserActivityCounts](../resources/teamsuseractivitycounts.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_teamsuseractivitycounts"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/teamsUserActivityCounts
Content-Type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.teamsUserActivityCounts",
  "calls": "Integer",
  "meetings": "Integer",
  "privateChatMessages": "Integer",
  "reportDate": "Date",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "teamChatMessages": "Integer"
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
  "@odata.type": "#microsoft.graph.teamsUserActivityCounts",
  "id": "367fde21-de21-367f-21de-7f3621de7f36",
  "calls": "Integer",
  "meetings": "Integer",
  "privateChatMessages": "Integer",
  "reportDate": "Date",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "teamChatMessages": "Integer"
}
```


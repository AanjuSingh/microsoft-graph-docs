---
title: "Create teamsUserActivityDistributionUserCounts"
description: "Create a new teamsUserActivityDistributionUserCounts object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create teamsUserActivityDistributionUserCounts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object.

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
POST ** Collection URI for microsoft.graph.teamsUserActivityDistributionUserCounts not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object.

The following table shows the properties that are required when you create the [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|calls|Int64|**TODO: Add Description**|
|meetings|Int64|**TODO: Add Description**|
|privateChatMessages|Int64|**TODO: Add Description**|
|reportPeriod|String|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|teamChatMessages|Int64|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [teamsUserActivityDistributionUserCounts](../resources/teamsuseractivitydistributionusercounts.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_teamsuseractivitydistributionusercounts_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.teamsUserActivityDistributionUserCounts not found
Content-Type: application/json
Content-length: 262

{
  "@odata.type": "#microsoft.graph.teamsUserActivityDistributionUserCounts",
  "calls": "Integer",
  "meetings": "Integer",
  "privateChatMessages": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "teamChatMessages": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityDistributionUserCounts"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.teamsUserActivityDistributionUserCounts",
  "id": "803e1eb5-1eb5-803e-b51e-3e80b51e3e80",
  "calls": "Integer",
  "meetings": "Integer",
  "privateChatMessages": "Integer",
  "reportPeriod": "String",
  "reportRefreshDate": "Date",
  "teamChatMessages": "Integer"
}
```


---
title: "Update meetingActivityStatistics"
description: "Update the properties of a meetingActivityStatistics object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update meetingActivityStatistics
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.

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
PATCH /meetingActivityStatistics
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object.

The following table shows the properties that are required when you update the [meetingActivityStatistics](../resources/meetingactivitystatistics.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activity|analyticsActivityType|**TODO: Add Description** Inherited from [activityStatistics](../resources/activitystatistics.md). Possible values are: `Email`, `Meeting`, `Focus`, `Chat`, `Call`.|
|duration|Duration|**TODO: Add Description** Inherited from [activityStatistics](../resources/activitystatistics.md)|
|endDate|Date|**TODO: Add Description** Inherited from [activityStatistics](../resources/activitystatistics.md)|
|startDate|Date|**TODO: Add Description** Inherited from [activityStatistics](../resources/activitystatistics.md)|
|timeZoneUsed|String|**TODO: Add Description** Inherited from [activityStatistics](../resources/activitystatistics.md)|
|afterHours|Duration|**TODO: Add Description**|
|conflicting|Duration|**TODO: Add Description**|
|long|Duration|**TODO: Add Description**|
|multitasking|Duration|**TODO: Add Description**|
|organized|Duration|**TODO: Add Description**|
|recurring|Duration|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [meetingActivityStatistics](../resources/meetingactivitystatistics.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_meetingactivitystatistics"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/meetingActivityStatistics
Content-Type: application/json
Content-length: 426

{
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "activity": "String",
  "duration": "String (duration)",
  "endDate": "Date",
  "startDate": "Date",
  "timeZoneUsed": "String",
  "afterHours": "String (duration)",
  "conflicting": "String (duration)",
  "long": "String (duration)",
  "multitasking": "String (duration)",
  "organized": "String (duration)",
  "recurring": "String (duration)"
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
  "@odata.type": "#microsoft.graph.meetingActivityStatistics",
  "id": "0e9bb964-b964-0e9b-64b9-9b0e64b99b0e",
  "activity": "String",
  "duration": "String (duration)",
  "endDate": "Date",
  "startDate": "Date",
  "timeZoneUsed": "String",
  "afterHours": "String (duration)",
  "conflicting": "String (duration)",
  "long": "String (duration)",
  "multitasking": "String (duration)",
  "organized": "String (duration)",
  "recurring": "String (duration)"
}
```


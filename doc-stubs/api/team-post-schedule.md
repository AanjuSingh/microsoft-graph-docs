---
title: "Create schedule"
description: "Create a new schedule object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create schedule
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new schedule object.

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
POST /team/schedule
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [schedule](../resources/schedule.md) object.

The following table shows the properties that are required when you create the [schedule](../resources/schedule.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description**|
|enabled|Boolean|**TODO: Add Description**|
|timeZone|String|**TODO: Add Description**|
|provisionStatus|operationStatus|**TODO: Add Description**. The possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.|
|provisionStatusCode|String|**TODO: Add Description**|
|workforceIntegrationIds|String collection|**TODO: Add Description**|
|timeClockEnabled|Boolean|**TODO: Add Description**|
|timeClockSettings|[Microsoft.Teams.Shifts.timeClockSettings](../resources/timeclocksettings.md)|**TODO: Add Description**|
|openShiftsEnabled|Boolean|**TODO: Add Description**|
|swapShiftsRequestsEnabled|Boolean|**TODO: Add Description**|
|offerShiftRequestsEnabled|Boolean|**TODO: Add Description**|
|timeOffRequestsEnabled|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [schedule](../resources/schedule.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_schedule_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/team/schedule
Content-Type: application/json
Content-length: 510

{
  "@odata.type": "#Microsoft.Teams.Shifts.schedule",
  "enabled": "Boolean",
  "timeZone": "String",
  "provisionStatus": "String",
  "provisionStatusCode": "String",
  "workforceIntegrationIds": [
    "String"
  ],
  "timeClockEnabled": "Boolean",
  "timeClockSettings": {
    "@odata.type": "microsoft.graph.timeClockSettings"
  },
  "openShiftsEnabled": "Boolean",
  "swapShiftsRequestsEnabled": "Boolean",
  "offerShiftRequestsEnabled": "Boolean",
  "timeOffRequestsEnabled": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.Teams.Shifts.schedule"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.Teams.Shifts.schedule",
  "id": "83a29188-9188-83a2-8891-a2838891a283",
  "enabled": "Boolean",
  "timeZone": "String",
  "provisionStatus": "String",
  "provisionStatusCode": "String",
  "workforceIntegrationIds": [
    "String"
  ],
  "timeClockEnabled": "Boolean",
  "timeClockSettings": {
    "@odata.type": "microsoft.graph.timeClockSettings"
  },
  "openShiftsEnabled": "Boolean",
  "swapShiftsRequestsEnabled": "Boolean",
  "offerShiftRequestsEnabled": "Boolean",
  "timeOffRequestsEnabled": "Boolean"
}
```


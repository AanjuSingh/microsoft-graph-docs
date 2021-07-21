---
title: "List events"
description: "Get the event resources from the events navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List events
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the event resources from the events navigation property.

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
GET /me/events
GET /users/{usersId}/events
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [event](../resources/event.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_event"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/events
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.event)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.event",
      "id": "c435642b-642b-c435-2b64-35c42b6435c4",
      "categories": [
        "String"
      ],
      "changeKey": "String",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "allowNewTimeProposals": "Boolean",
      "attendees": [
        {
          "@odata.type": "microsoft.graph.attendee"
        }
      ],
      "body": {
        "@odata.type": "microsoft.graph.itemBody"
      },
      "bodyPreview": "String",
      "cancelledOccurrences": [
        "String"
      ],
      "end": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "hasAttachments": "Boolean",
      "hideAttendees": "Boolean",
      "importance": "String",
      "isAllDay": "Boolean",
      "isCancelled": "Boolean",
      "isDraft": "Boolean",
      "isOnlineMeeting": "Boolean",
      "isOrganizer": "Boolean",
      "isReminderOn": "Boolean",
      "location": {
        "@odata.type": "microsoft.graph.location"
      },
      "locations": [
        {
          "@odata.type": "microsoft.graph.location"
        }
      ],
      "occurrenceId": "String",
      "onlineMeeting": {
        "@odata.type": "microsoft.graph.onlineMeetingInfo"
      },
      "onlineMeetingProvider": "String",
      "onlineMeetingUrl": "String",
      "organizer": {
        "@odata.type": "microsoft.graph.recipient"
      },
      "originalEndTimeZone": "String",
      "originalStart": "String (timestamp)",
      "originalStartTimeZone": "String",
      "recurrence": {
        "@odata.type": "microsoft.graph.patternedRecurrence"
      },
      "reminderMinutesBeforeStart": "Integer",
      "responseRequested": "Boolean",
      "responseStatus": {
        "@odata.type": "microsoft.graph.responseStatus"
      },
      "sensitivity": "String",
      "seriesMasterId": "String",
      "showAs": "String",
      "start": {
        "@odata.type": "microsoft.graph.dateTimeTimeZone"
      },
      "subject": "String",
      "transactionId": "String",
      "type": "String",
      "uid": "String",
      "webLink": "String"
    }
  ]
}
```


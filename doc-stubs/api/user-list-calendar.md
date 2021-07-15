---
title: "List calendar"
description: "Get the calendar resources from the calendar navigation property."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List calendar
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get the calendar resources from the calendar navigation property.

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
GET /me/calendar
GET /users/{usersId}/calendar
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

If successful, this method returns a `200 OK` response code and a collection of [calendar](../resources/calendar.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_calendar"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/calendar
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.calendar)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.calendar",
      "id": "b0b0f208-f208-b0b0-08f2-b0b008f2b0b0",
      "allowedOnlineMeetingProviders": [
        "String"
      ],
      "calendarGroupId": "String",
      "canEdit": "Boolean",
      "canShare": "Boolean",
      "canViewPrivateItems": "Boolean",
      "changeKey": "String",
      "color": "String",
      "defaultOnlineMeetingProvider": "String",
      "hexColor": "String",
      "isDefaultCalendar": "Boolean",
      "isRemovable": "Boolean",
      "isShared": "Boolean",
      "isSharedWithMe": "Boolean",
      "isTallyingResponses": "Boolean",
      "name": "String",
      "owner": {
        "@odata.type": "microsoft.graph.emailAddress"
      }
    }
  ]
}
```


---
title: "Get bookingAppointment"
description: "Read the properties and relationships of a bookingAppointment object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get bookingAppointment
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [bookingAppointment](../resources/bookingappointment.md) object.

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
GET /bookingBusinesses/{bookingBusinessesId}/appointments/{bookingAppointmentId}
GET /bookingBusinesses/{bookingBusinessesId}/calendarView/{bookingAppointmentId}
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

If successful, this method returns a `200 OK` response code and a [bookingAppointment](../resources/bookingappointment.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_bookingappointment"
}
-->
``` http
GET https://graph.microsoft.com/beta/bookingBusinesses/{bookingBusinessesId}/appointments/{bookingAppointmentId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.bookingAppointment"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.bookingAppointment",
    "id": "5879a5d3-a5d3-5879-d3a5-7958d3a57958",
    "additionalInformation": "String",
    "customerEmailAddress": "String",
    "customerId": "String",
    "customerLocation": {
      "@odata.type": "microsoft.graph.location"
    },
    "customerName": "String",
    "customerNotes": "String",
    "customerPhone": "String",
    "duration": "String (duration)",
    "end": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "invoiceAmount": "Double",
    "invoiceDate": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    },
    "invoiceId": "String",
    "invoiceStatus": "String",
    "invoiceUrl": "String",
    "isLocationOnline": "Boolean",
    "onlineMeetingUrl": "String",
    "optOutOfCustomerEmail": "Boolean",
    "postBuffer": "String (duration)",
    "preBuffer": "String (duration)",
    "price": "Double",
    "priceType": "String",
    "reminders": [
      {
        "@odata.type": "microsoft.graph.bookingReminder"
      }
    ],
    "selfServiceAppointmentId": "String",
    "serviceId": "String",
    "serviceLocation": {
      "@odata.type": "microsoft.graph.location"
    },
    "serviceName": "String",
    "serviceNotes": "String",
    "staffMemberIds": [
      "String"
    ],
    "start": {
      "@odata.type": "microsoft.graph.dateTimeTimeZone"
    }
  }
}
```


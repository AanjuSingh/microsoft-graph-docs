---
title: "bookingReminder resource type"
description: "This type represents when and to whom to send an e-mail reminder."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# bookingReminder resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

This type represents when and to whom to send an e-mail reminder.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|message|String|Message to send.|
|offset|Duration|How much time before an appointment the reminder should be sent.|
|recipients|bookingReminderRecipients|Who should receive the reminder. Possible values are: `allAttendees`, `staff`, `customer`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bookingReminder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bookingReminder",
  "message": "String",
  "offset": "String (duration)",
  "recipients": "String"
}
```


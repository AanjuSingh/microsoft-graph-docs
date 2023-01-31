---
title: "pstnOnlineMeetingDialoutReport resource type"
description: "Represents a report of usage and money spent for the audio conferencing dial-out service over a selected period"
author: "radoslag"
ms.localizationpriority: medium
ms.prod: "cloud-communications"
doc_type: resourcePageType
---

# pstnOnlineMeetingDialoutReport resource type

Namespace: microsoft.graph.callRecords

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents a report of usage and money spent for the audio conferencing dial-out service over a selected period.
The report is aggregated by user, user location, destination context (domestic/international), currency.

All dial-out calls/duration/charge is counted under a meeting organizer. It's not necessarily the same person who dialed out.

## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [getPstnOnlineMeetingDialoutReport](../api/callrecords-callrecord-getpstnonlinemeetingdialoutreport.md) | [microsoft.graph.callRecords.pstnOnlineMeetingDialoutReport collection](callrecords-pstnonlinemeetingdialoutreport.md) | Get aggregated report of usage and money spent for the audio conferencing dial-out service |

## Properties

|Property|Type|Description|
|:---|:---|:---|
|currency|String|Currency used to calculate the cost of the call ([ISO 4217](https://en.wikipedia.org/wiki/ISO_4217))|
|destinationContext|String|Whether the call was `Domestic` (within a country or region) or `International` (outside a country or region) based on the user's location|
|totalCallCharge|Double|Total costs of all the calls within the selected time range (includes call charges and connection fees)|
|totalCalls|Int32|Total number of dial-out calls within the selected time range|
|totalCallSeconds|Int32|Total duration of all the calls within the selected time range, in seconds|
|usageLocation|String|Country code of the user ([ISO 3166-1 alpha-2](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2))|
|userDisplayName|String|Display name of the user|
|userId|String|User Id in Graph (GUID)|
|userPrincipalName|String|UserPrincipalName (sign-in name) in Azure Active Directory. This is usually the same as user's SIP Address, and can be same as user's e-mail address|

## Relationships

None.

## JSON representation

The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.callRecords.pstnOnlineMeetingDialoutReport"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.callRecords.pstnOnlineMeetingDialoutReport",
  "userId": "String",
  "userPrincipalName": "String",
  "userDisplayName": "String",
  "usageLocation": "String",
  "destinationContext": "String",
  "currency": "String",
  "totalCalls": "Integer",
  "totalCallCharge": "Double",
  "totalCallSeconds": "Integer"
}
```

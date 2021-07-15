---
title: "overallPrintUsageSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# overallPrintUsageSummary resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|activePrintersCount|Int32|**TODO: Add Description**|
|activeUsersCount|Int32|**TODO: Add Description**|
|daysInPeriod|Int32|**TODO: Add Description**|
|topPrinters|[printerUsageSummary](../resources/printerusagesummary.md) collection|**TODO: Add Description**|
|topUsers|[userPrintUsageSummary](../resources/userprintusagesummary.md) collection|**TODO: Add Description**|
|totalIncompleteJobs|Int32|**TODO: Add Description**|
|totalJobsProcessed|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.overallPrintUsageSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.overallPrintUsageSummary",
  "activePrintersCount": "Integer",
  "activeUsersCount": "Integer",
  "daysInPeriod": "Integer",
  "topPrinters": [
    {
      "@odata.type": "microsoft.graph.printerUsageSummary"
    }
  ],
  "topUsers": [
    {
      "@odata.type": "microsoft.graph.userPrintUsageSummary"
    }
  ],
  "totalIncompleteJobs": "Integer",
  "totalJobsProcessed": "Integer"
}
```


---
title: "searchHitsContainer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# searchHitsContainer resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|aggregations|[searchAggregation](../resources/searchaggregation.md) collection|**TODO: Add Description**|
|hits|[searchHit](../resources/searchhit.md) collection|**TODO: Add Description**|
|moreResultsAvailable|Boolean|**TODO: Add Description**|
|total|Int32|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchHitsContainer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchHitsContainer",
  "aggregations": [
    {
      "@odata.type": "microsoft.graph.searchAggregation"
    }
  ],
  "hits": [
    {
      "@odata.type": "microsoft.graph.searchHit"
    }
  ],
  "moreResultsAvailable": "Boolean",
  "total": "Integer"
}
```


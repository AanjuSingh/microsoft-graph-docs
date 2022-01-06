---
title: "searchResultSet resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# searchResultSet resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|hitsContainers|[searchHitsContainer](../resources/searchhitscontainer.md) collection|**TODO: Add Description**|
|resultTemplates|[resultTemplateDictionary](../resources/resulttemplatedictionary.md)|**TODO: Add Description**|
|searchTerms|String collection|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.searchResultSet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.searchResultSet",
  "searchTerms": [
    "String"
  ],
  "hitsContainers": [
    {
      "@odata.type": "microsoft.graph.searchHitsContainer"
    }
  ],
  "resultTemplates": {
    "@odata.type": "microsoft.graph.resultTemplateDictionary"
  }
}
```


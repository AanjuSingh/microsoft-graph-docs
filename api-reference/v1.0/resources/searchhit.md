---
title: "searchHit resource type"
description: "Description of searchHit entity"
ms.localizationpriority: medium
author: "nmoreau"
ms.prod: "search"
doc_type: "resourcePageType"
---

# searchHit resource type

Namespace: microsoft.graph

Represents a single result within the list of search results.

## Properties

| Property     | Type        | Description |
|:-------------|:------------|:------------|
|contentSource|String|The name of the content source which the **externalItem** is part of .|
|hitId|String|The internal identifier for the item.|
|rank|Int32|The rank or the order of the result.|
|resultTemplateId|String|ID of the result template used to render the search result. This ID must map to a display layout in the **resultTemplates** dictionary that is also included in the [searchResponse](searchresponse.md).|
|resource|[entity](entity.md)|The underlying Microsoft Graph representation of the search result.|
|summary|String|A summary of the result, if a summary is available.|

## JSON representation

The following is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.searchHit",
  "baseType": null
}-->

```json
{
  "contentSource": "String",
  "hitId": "String",
  "rank": "Int32",
  "resultTemplateId": "String",
  "resource": { "@odata.type": "microsoft.graph.entity" },
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "searchHit resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


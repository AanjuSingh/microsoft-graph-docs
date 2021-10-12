---
title: "siteSource resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# siteSource resource type

Namespace: microsoft.graph.ediscovery



**TODO: Add Description**


Inherits from [dataSource](../resources/ediscovery-datasource.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List siteSources](../api/ediscovery-sitesource-list.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection|Get a list of the [siteSource](../resources/ediscovery-sitesource.md) objects and their properties.|
|[Create siteSource](../api/ediscovery-sitesource-create.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Create a new [siteSource](../resources/ediscovery-sitesource.md) object.|
|[Get siteSource](../api/ediscovery-sitesource-get.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Read the properties and relationships of a [siteSource](../resources/ediscovery-sitesource.md) object.|
|[Update siteSource](../api/ediscovery-sitesource-update.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Update the properties of a [siteSource](../resources/ediscovery-sitesource.md) object.|
|[Delete siteSource](../api/ediscovery-sitesource-delete.md)|None|Deletes a [siteSource](../resources/ediscovery-sitesource.md) object.|
|[List site](../api/ediscovery-sitesource-list-site.md)|[microsoft.graph.site](../resources/ediscovery-site.md) collection|Get the site resources from the site navigation property.|
|[Add site](../api/ediscovery-sitesource-post-site.md)|[microsoft.graph.site](../resources/ediscovery-site.md)|Add site by posting to the site collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description** Inherited from [dataSource](../resources/ediscovery-datasource.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [dataSource](../resources/ediscovery-datasource.md).|
|displayName|String|**TODO: Add Description** Inherited from [dataSource](../resources/ediscovery-datasource.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|site|[site](../resources/ediscovery-site.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "id": "String (identifier)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  }
}
```


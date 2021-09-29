---
title: "sourceCollection resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# sourceCollection resource type

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/ediscovery-entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List sourceCollections](../api/ediscovery-sourcecollection-list.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md) collection|Get a list of the [sourceCollection](../resources/ediscovery-sourcecollection.md) objects and their properties.|
|[Create sourceCollection](../api/ediscovery-sourcecollection-create.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Create a new [sourceCollection](../resources/ediscovery-sourcecollection.md) object.|
|[Get sourceCollection](../api/ediscovery-sourcecollection-get.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Read the properties and relationships of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.|
|[Update sourceCollection](../api/ediscovery-sourcecollection-update.md)|[microsoft.graph.ediscovery.sourceCollection](../resources/ediscovery-sourcecollection.md)|Update the properties of a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.|
|[Delete sourceCollection](../api/ediscovery-sourcecollection-delete.md)|None|Deletes a [sourceCollection](../resources/ediscovery-sourcecollection.md) object.|
|[estimateStatistics](../api/ediscovery-sourcecollection-estimatestatistics.md)|None|**TODO: Add Description**|
|[List additionalSources](../api/ediscovery-sourcecollection-list-additionalsources.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection|Get the dataSource resources from the additionalSources navigation property.|
|[Create dataSource](../api/ediscovery-sourcecollection-post-additionalsources.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Create a new dataSource object.|
|[List addToReviewSetOperation](../api/ediscovery-sourcecollection-list-addtoreviewsetoperation.md)|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md) collection|Get the addToReviewSetOperation resources from the addToReviewSetOperation navigation property.|
|[Add addToReviewSetOperation](../api/ediscovery-sourcecollection-post-addtoreviewsetoperation.md)|[microsoft.graph.ediscovery.addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|Add addToReviewSetOperation by posting to the addToReviewSetOperation collection.|
|[List custodianSources](../api/ediscovery-sourcecollection-list-custodiansources.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection|Get the dataSource resources from the custodianSources navigation property.|
|[Add dataSource](../api/ediscovery-sourcecollection-post-custodiansources.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|Add custodianSources by posting to the custodianSources collection.|
|[List estimateStatisticsOperation](../api/ediscovery-sourcecollection-list-lastestimatestatisticsoperation.md)|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md) collection|Get the estimateStatisticsOperation resources from the lastEstimateStatisticsOperation navigation property.|
|[Add estimateStatisticsOperation](../api/ediscovery-sourcecollection-post-lastestimatestatisticsoperation.md)|[microsoft.graph.ediscovery.estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|Add lastEstimateStatisticsOperation by posting to the lastEstimateStatisticsOperation collection.|
|[List noncustodialSources](../api/ediscovery-sourcecollection-list-noncustodialsources.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) collection|Get the noncustodialDataSource resources from the noncustodialSources navigation property.|
|[Add noncustodialDataSource](../api/ediscovery-sourcecollection-post-noncustodialsources.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|Add noncustodialSources by posting to the noncustodialSources collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|contentQuery|String|**TODO: Add Description**|
|createdBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description**|
|createdDateTime|DateTimeOffset|**TODO: Add Description**|
|dataSourceScopes|dataSourceScopes|**TODO: Add Description**. The possible values are: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`, `unknownFutureValue`.|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/ediscovery-entity.md).|
|lastModifiedBy|[microsoft.graph.identitySet](../resources/ediscovery-identityset.md)|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|additionalSources|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection|**TODO: Add Description**|
|addToReviewSetOperation|[addToReviewSetOperation](../resources/ediscovery-addtoreviewsetoperation.md)|**TODO: Add Description**|
|custodianSources|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) collection|**TODO: Add Description**|
|lastEstimateStatisticsOperation|[estimateStatisticsOperation](../resources/ediscovery-estimatestatisticsoperation.md)|**TODO: Add Description**|
|noncustodialSources|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.sourceCollection",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.sourceCollection",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "contentQuery": "String",
  "dataSourceScopes": "String"
}
```


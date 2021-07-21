---
title: "userExperienceAnalyticsBaseline resource type"
description: "The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# userExperienceAnalyticsBaseline resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The user experience analytics baseline entity contains baseline values against which to compare the user experience analytics scores.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List userExperienceAnalyticsBaselines](../api/userexperienceanalyticsbaseline-list.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) collection|Get a list of the [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) objects and their properties.|
|[Create userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-create.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Create a new [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[Get userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-get.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Read the properties and relationships of a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[Update userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-update.md)|[userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md)|Update the properties of a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[Delete userExperienceAnalyticsBaseline](../api/userexperienceanalyticsbaseline-delete.md)|None|Deletes a [userExperienceAnalyticsBaseline](../resources/userexperienceanalyticsbaseline.md) object.|
|[List userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-list-apphealthmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategory resources from the appHealthMetrics navigation property.|
|[Add userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-post-apphealthmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add appHealthMetrics by posting to the appHealthMetrics collection.|
|[List userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-list-bestpracticesmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategory resources from the bestPracticesMetrics navigation property.|
|[Add userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-post-bestpracticesmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add bestPracticesMetrics by posting to the bestPracticesMetrics collection.|
|[List userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-list-devicebootperformancemetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategory resources from the deviceBootPerformanceMetrics navigation property.|
|[Add userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-post-devicebootperformancemetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add deviceBootPerformanceMetrics by posting to the deviceBootPerformanceMetrics collection.|
|[List userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-list-rebootanalyticsmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategory resources from the rebootAnalyticsMetrics navigation property.|
|[Add userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-post-rebootanalyticsmetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add rebootAnalyticsMetrics by posting to the rebootAnalyticsMetrics collection.|
|[List userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-list-resourceperformancemetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategory resources from the resourcePerformanceMetrics navigation property.|
|[Add userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-post-resourceperformancemetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add resourcePerformanceMetrics by posting to the resourcePerformanceMetrics collection.|
|[List userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-list-workfromanywheremetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md) collection|Get the userExperienceAnalyticsCategory resources from the workFromAnywhereMetrics navigation property.|
|[Add userExperienceAnalyticsCategory](../api/userexperienceanalyticsbaseline-post-workfromanywheremetrics.md)|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|Add workFromAnywhereMetrics by posting to the workFromAnywhereMetrics collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date the custom baseline was created.|
|displayName|String|The name of the user experience analytics baseline.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isBuiltIn|Boolean|Signifies if the current baseline is the commercial median baseline or a custom baseline.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appHealthMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics app health metrics.|
|bestPracticesMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics best practices metrics.|
|deviceBootPerformanceMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics device boot performance metrics.|
|rebootAnalyticsMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics reboot analytics metrics.|
|resourcePerformanceMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics resource performance metrics.|
|workFromAnywhereMetrics|[userExperienceAnalyticsCategory](../resources/userexperienceanalyticscategory.md)|The user experience analytics work from anywhere metrics.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsBaseline",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsBaseline",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "isBuiltIn": "Boolean"
}
```


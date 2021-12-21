---
title: "deviceManagementReports resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementReports resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceManagementReports](../api/intune-devicemanagementreports-list.md)|[deviceManagementReports](../resources/intune-devicemanagementreports.md) collection|Get a list of the [deviceManagementReports](../resources/intune-devicemanagementreports.md) objects and their properties.|
|[Create deviceManagementReports](../api/devicemanagement-post-reports.md)|[deviceManagementReports](../resources/intune-devicemanagementreports.md)|Create a new [deviceManagementReports](../resources/intune-devicemanagementreports.md) object.|
|[Get deviceManagementReports](../api/intune-devicemanagementreports-get.md)|[deviceManagementReports](../resources/intune-devicemanagementreports.md)|Read the properties and relationships of a [deviceManagementReports](../resources/intune-devicemanagementreports.md) object.|
|[Update deviceManagementReports](../api/intune-devicemanagementreports-update.md)|[deviceManagementReports](../resources/intune-devicemanagementreports.md)|Update the properties of a [deviceManagementReports](../resources/intune-devicemanagementreports.md) object.|
|[Delete deviceManagementReports](../api/intune-devicemanagementreports-delete.md)|None|Deletes a [deviceManagementReports](../resources/intune-devicemanagementreports.md) object.|
|[getQuietTimePolicyUsersReport](../api/intune-devicemanagementreports-getquiettimepolicyusersreport.md)|Stream|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|cachedReportConfigurations|[deviceManagementCachedReportConfiguration](../resources/intune-devicemanagementcachedreportconfiguration.md) collection|**TODO: Add Description**|
|exportJobs|[deviceManagementExportJob](../resources/intune-devicemanagementexportjob.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementReports",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "String (identifier)"
}
```


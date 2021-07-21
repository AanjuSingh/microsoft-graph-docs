---
title: "printer resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# printer resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [printerBase](../resources/printerbase.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List printers](../api/printer-list.md)|[printer](../resources/printer.md) collection|Get a list of the [printer](../resources/printer.md) objects and their properties.|
|[Create printer](../api/printer-create.md)|[printer](../resources/printer.md)|Create a new [printer](../resources/printer.md) object.|
|[Get printer](../api/printer-get.md)|[printer](../resources/printer.md)|Read the properties and relationships of a [printer](../resources/printer.md) object.|
|[Update printer](../api/printer-update.md)|[printer](../resources/printer.md)|Update the properties of a [printer](../resources/printer.md) object.|
|[Delete printer](../api/printer-delete.md)|None|Deletes a [printer](../resources/printer.md) object.|
|[create](../api/printer-create.md)|None|**TODO: Add Description**|
|[resetDefaults](../api/printer-resetdefaults.md)|None|**TODO: Add Description**|
|[restoreFactoryDefaults](../api/printer-restorefactorydefaults.md)|None|**TODO: Add Description**|
|[getCapabilities](../api/printer-getcapabilities.md)|[printerCapabilities](../resources/printercapabilities.md)|**TODO: Add Description**|
|[List connectors](../api/printer-list-connectors.md)|[printConnector](../resources/printconnector.md) collection|Get the printConnector resources from the connectors navigation property.|
|[Add printConnector](../api/printer-post-connectors.md)|[printConnector](../resources/printconnector.md)|Add connectors by posting to the connectors collection.|
|[List jobs](../api/printer-list-jobs.md)|[printJob](../resources/printjob.md) collection|Get the printJob resources from the jobs navigation property.|
|[Create printJob](../api/printer-post-jobs.md)|[printJob](../resources/printjob.md)|Create a new printJob object.|
|[List printerShare](../api/printer-list-share.md)|[printerShare](../resources/printershare.md) collection|Get the printerShare resources from the share navigation property.|
|[Add printerShare](../api/printer-post-share.md)|[printerShare](../resources/printershare.md)|Add share by posting to the share collection.|
|[List shares](../api/printer-list-shares.md)|[printerShare](../resources/printershare.md) collection|Get the printerShare resources from the shares navigation property.|
|[Add printerShare](../api/printer-post-shares.md)|[printerShare](../resources/printershare.md)|Add shares by posting to the shares collection.|
|[List taskTriggers](../api/printer-list-tasktriggers.md)|[printTaskTrigger](../resources/printtasktrigger.md) collection|Get the printTaskTrigger resources from the taskTriggers navigation property.|
|[Create printTaskTrigger](../api/printer-post-tasktriggers.md)|[printTaskTrigger](../resources/printtasktrigger.md)|Create a new printTaskTrigger object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|acceptingJobs|Boolean|**TODO: Add Description**|
|capabilities|[printerCapabilities](../resources/printercapabilities.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|defaults|[printerDefaults](../resources/printerdefaults.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|displayName|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|hasPhysicalDevice|Boolean|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isAcceptingJobs|Boolean|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|isShared|Boolean|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|location|[printerLocation](../resources/printerlocation.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|manufacturer|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|model|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|name|String|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|
|registeredDateTime|DateTimeOffset|**TODO: Add Description**|
|status|[printerStatus](../resources/printerstatus.md)|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md).|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|connectors|[printConnector](../resources/printconnector.md) collection|**TODO: Add Description**|
|jobs|[printJob](../resources/printjob.md) collection|**TODO: Add Description** Inherited from [printerBase](../resources/printerbase.md)|
|share|[printerShare](../resources/printershare.md)|**TODO: Add Description**|
|shares|[printerShare](../resources/printershare.md) collection|**TODO: Add Description**|
|taskTriggers|[printTaskTrigger](../resources/printtasktrigger.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printer",
  "baseType": "microsoft.graph.printerBase",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printer",
  "id": "String (identifier)",
  "capabilities": {
    "@odata.type": "microsoft.graph.printerCapabilities"
  },
  "defaults": {
    "@odata.type": "microsoft.graph.printerDefaults"
  },
  "displayName": "String",
  "isAcceptingJobs": "Boolean",
  "location": {
    "@odata.type": "microsoft.graph.printerLocation"
  },
  "manufacturer": "String",
  "model": "String",
  "name": "String",
  "status": {
    "@odata.type": "microsoft.graph.printerStatus"
  },
  "acceptingJobs": "Boolean",
  "hasPhysicalDevice": "Boolean",
  "isShared": "Boolean",
  "lastSeenDateTime": "String (timestamp)",
  "registeredDateTime": "String (timestamp)"
}
```


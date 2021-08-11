---
title: "deviceManagementScriptAssignment resource type"
description: "Contains properties used to assign a device management script to a group."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementScriptAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contains properties used to assign a device management script to a group.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceManagementScriptAssignments](../api/devicemanagementscriptassignment-list.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) collection|Get a list of the [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) objects and their properties.|
|[Create deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-create.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Create a new [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|
|[Get deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-get.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Read the properties and relationships of a [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|
|[Update deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-update.md)|[deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md)|Update the properties of a [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|
|[Delete deviceManagementScriptAssignment](../api/devicemanagementscriptassignment-delete.md)|None|Deletes a [deviceManagementScriptAssignment](../resources/devicemanagementscriptassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|Key of the device management script group assignment entity. This property is read-only.|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The Id of the Azure Active Directory group we are targeting the script to.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementScriptAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementScriptAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```


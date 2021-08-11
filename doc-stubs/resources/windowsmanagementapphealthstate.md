---
title: "windowsManagementAppHealthState resource type"
description: "Windows management app health state entity."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsManagementAppHealthState resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Windows management app health state entity.

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List windowsManagementAppHealthStates](../api/windowsmanagementapphealthstate-list.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) collection|Get a list of the [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) objects and their properties.|
|[Create windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-create.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Create a new [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[Get windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-get.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Read the properties and relationships of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[Update windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-update.md)|[windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md)|Update the properties of a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|
|[Delete windowsManagementAppHealthState](../api/windowsmanagementapphealthstate-delete.md)|None|Deletes a [windowsManagementAppHealthState](../resources/windowsmanagementapphealthstate.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|deviceName|String|Name of the device on which Windows management app is installed.|
|deviceOSVersion|String|Windows 10 OS version of the device on which Windows management app is installed.|
|healthState|healthState|Windows management app health state. Possible values are: `unknown`, `healthy`, `unhealthy`.|
|id|String|Unique Identifier for the Windows management app health state. This property is read-only.|
|installedVersion|String|Windows management app installed version.|
|lastCheckInDateTime|DateTimeOffset|Windows management app last check-in time.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsManagementAppHealthState",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
  "id": "String (identifier)",
  "healthState": "String",
  "installedVersion": "String",
  "lastCheckInDateTime": "String (timestamp)",
  "deviceName": "String",
  "deviceOSVersion": "String"
}
```


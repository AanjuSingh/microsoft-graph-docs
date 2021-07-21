---
title: "windowsInformationProtectionWipeAction resource type"
description: "Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# windowsInformationProtectionWipeAction resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List windowsInformationProtectionWipeActions](../api/windowsinformationprotectionwipeaction-list.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) collection|Get a list of the [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) objects and their properties.|
|[Create windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-create.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Create a new [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[Get windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-get.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Read the properties and relationships of a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[Update windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-update.md)|[windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md)|Update the properties of a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|
|[Delete windowsInformationProtectionWipeAction](../api/windowsinformationprotectionwipeaction-delete.md)|None|Deletes a [windowsInformationProtectionWipeAction](../resources/windowsinformationprotectionwipeaction.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastCheckInDateTime|DateTimeOffset|Last checkin time of the device that was targeted by this wipe action.|
|status|actionState|Wipe action status. Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.|
|targetedDeviceMacAddress|String|Targeted device Mac address.|
|targetedDeviceName|String|Targeted device name.|
|targetedDeviceRegistrationId|String|The DeviceRegistrationId being targeted by this wipe action.|
|targetedUserId|String|The UserId being targeted by this wipe action.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "lastCheckInDateTime": "String (timestamp)",
  "status": "String",
  "targetedDeviceMacAddress": "String",
  "targetedDeviceName": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedUserId": "String"
}
```


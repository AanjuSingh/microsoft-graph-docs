---
title: "deviceConfigurationDeviceStatus resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceConfigurationDeviceStatus resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-list.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) collection|Get a list of the [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) objects and their properties.|
|[Create deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-create.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Create a new [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[Get deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-get.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Read the properties and relationships of a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[Update deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-update.md)|[deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md)|Update the properties of a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|
|[Delete deviceConfigurationDeviceStatus](../api/deviceconfigurationdevicestatus-delete.md)|None|Deletes a [deviceConfigurationDeviceStatus](../resources/deviceconfigurationdevicestatus.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|complianceGracePeriodExpirationDateTime|DateTimeOffset|The DateTime when device compliance grace period expires|
|deviceDisplayName|String|Device name of the DevicePolicyStatus.|
|deviceModel|String|The device model that is being reported|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|platform|Int32|Platform of the device that is being reported|
|status|complianceStatus|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userName|String|The User Name that is being reported|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationDeviceStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationDeviceStatus",
  "id": "String (identifier)",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "deviceDisplayName": "String",
  "deviceModel": "String",
  "lastReportedDateTime": "String (timestamp)",
  "platform": "Integer",
  "status": "String",
  "userName": "String",
  "userPrincipalName": "String"
}
```


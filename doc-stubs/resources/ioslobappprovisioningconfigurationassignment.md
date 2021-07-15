---
title: "iosLobAppProvisioningConfigurationAssignment resource type"
description: "A class containing the properties used for Group Assignment of an iOS LOB App Provisioning and Configuration."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# iosLobAppProvisioningConfigurationAssignment resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

A class containing the properties used for Group Assignment of an iOS LOB App Provisioning and Configuration.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List iosLobAppProvisioningConfigurationAssignments](../api/ioslobappprovisioningconfigurationassignment-list.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) collection|Get a list of the [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) objects and their properties.|
|[Create iosLobAppProvisioningConfigurationAssignment](../api/ioslobappprovisioningconfigurationassignment-create.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Create a new [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) object.|
|[Get iosLobAppProvisioningConfigurationAssignment](../api/ioslobappprovisioningconfigurationassignment-get.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Read the properties and relationships of an [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) object.|
|[Update iosLobAppProvisioningConfigurationAssignment](../api/ioslobappprovisioningconfigurationassignment-update.md)|[iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md)|Update the properties of an [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) object.|
|[Delete iosLobAppProvisioningConfigurationAssignment](../api/ioslobappprovisioningconfigurationassignment-delete.md)|None|Deletes an [iosLobAppProvisioningConfigurationAssignment](../resources/ioslobappprovisioningconfigurationassignment.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|target|[deviceAndAppManagementAssignmentTarget](../resources/deviceandappmanagementassignmenttarget.md)|The target group assignment defined by the admin.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosLobAppProvisioningConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```


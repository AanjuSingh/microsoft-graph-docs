---
title: "deviceManagementAbstractComplexSettingDefinition resource type"
description: "Entity representing the defintion for an abstract complex setting"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementAbstractComplexSettingDefinition resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Entity representing the defintion for an abstract complex setting


Inherits from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List deviceManagementAbstractComplexSettingDefinitions](../api/devicemanagementabstractcomplexsettingdefinition-list.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) collection|Get a list of the [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) objects and their properties.|
|[Create deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-create.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md)|Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|
|[Get deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-get.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md)|Read the properties and relationships of a [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|
|[Update deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-update.md)|[deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md)|Update the properties of a [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|
|[Delete deviceManagementAbstractComplexSettingDefinition](../api/devicemanagementabstractcomplexsettingdefinition-delete.md)|None|Deletes a [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection|Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection|Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|description|String|The setting's description Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|displayName|String|The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|documentationUrl|String|Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|headerSubtitle|String|subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|headerTitle|String|title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|implementations|String collection|List of definition IDs for all possible implementations of this abstract complex setting|
|isTopLevel|Boolean|If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|keywords|String collection|Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|placeholderText|String|Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md).|
|valueType|deviceManangementIntentValueType|The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md). Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "baseType": "microsoft.graph.deviceManagementSettingDefinition",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "String (identifier)",
  "constraints": [
    {
      "@odata.type": "microsoft.graph.deviceManagementEnumConstraint"
    }
  ],
  "dependencies": [
    {
      "@odata.type": "microsoft.graph.deviceManagementSettingDependency"
    }
  ],
  "description": "String",
  "displayName": "String",
  "documentationUrl": "String",
  "headerSubtitle": "String",
  "headerTitle": "String",
  "isTopLevel": "Boolean",
  "keywords": [
    "String"
  ],
  "placeholderText": "String",
  "valueType": "String",
  "implementations": [
    "String"
  ]
}
```


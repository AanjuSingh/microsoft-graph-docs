---
title: "Create deviceManagementAbstractComplexSettingDefinition"
description: "Create a new deviceManagementAbstractComplexSettingDefinition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceManagementAbstractComplexSettingDefinition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.graph.deviceManagementAbstractComplexSettingDefinition not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object.

The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|constraints|[deviceManagementConstraint](../resources/devicemanagementconstraint.md) collection|Collection of constraints for the setting value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|dependencies|[deviceManagementSettingDependency](../resources/devicemanagementsettingdependency.md) collection|Collection of dependencies on other settings Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|description|String|The setting's description Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|displayName|String|The setting's display name Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|documentationUrl|String|Url to setting documentation Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|headerSubtitle|String|subtitle of the setting header for more details about the category/section Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|headerTitle|String|title of the setting header represents a category/section of a setting/settings Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|isTopLevel|Boolean|If the setting is top level, it can be configured without the need to be wrapped in a collection or complex setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|keywords|String collection|Keywords associated with the setting Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|placeholderText|String|Placeholder text as an example of valid input Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md)|
|valueType|deviceManangementIntentValueType|The data type of the value Inherited from [deviceManagementSettingDefinition](../resources/devicemanagementsettingdefinition.md). Possible values are: `integer`, `boolean`, `string`, `complex`, `collection`, `abstractComplex`.|
|implementations|String collection|List of definition IDs for all possible implementations of this abstract complex setting|



## Response

If successful, this method returns a `201 Created` response code and a [deviceManagementAbstractComplexSettingDefinition](../resources/devicemanagementabstractcomplexsettingdefinition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementabstractcomplexsettingdefinition_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.deviceManagementAbstractComplexSettingDefinition not found
Content-Type: application/json
Content-length: 631

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
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


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingDefinition"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingDefinition",
  "id": "23bbe8cb-e8cb-23bb-cbe8-bb23cbe8bb23",
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


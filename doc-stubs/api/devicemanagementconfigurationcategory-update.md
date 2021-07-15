---
title: "Update deviceManagementConfigurationCategory"
description: "Update the properties of a deviceManagementConfigurationCategory object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagementConfigurationCategory
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceManagementConfigurationCategory](../resources/devicemanagementconfigurationcategory.md) object.

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
PATCH /deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementConfigurationCategory](../resources/devicemanagementconfigurationcategory.md) object.

The following table shows the properties that are required when you update the [deviceManagementConfigurationCategory](../resources/devicemanagementconfigurationcategory.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|childCategoryIds|String collection|List of child ids of the category.|
|description|String|Description of the item|
|displayName|String|Display name of the item|
|helpText|String|Help text of the item|
|name|String|Name of the item|
|parentCategoryId|String|Parent id of the category.|
|platforms|deviceManagementConfigurationPlatforms|Platforms types, which settings in the category have. Possible values are: `none`, `macOS`, `windows10X`, `windows10`.|
|rootCategoryId|String|Root id of the category.|
|settingUsage|deviceManagementConfigurationSettingUsage|Indicates that the category contains settings that are used for Compliance or Configuration. Possible values are: `none`, `configuration`.|
|technologies|deviceManagementConfigurationTechnologies|Technologies types, which settings in the category have. Possible values are: `none`, `mdm`, `windows10XManagement`, `configManager`, `microsoftSense`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementConfigurationCategory](../resources/devicemanagementconfigurationcategory.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementconfigurationcategory"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/configurationCategories/{deviceManagementConfigurationCategoryId}
Content-Type: application/json
Content-length: 374

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "childCategoryIds": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "helpText": "String",
  "name": "String",
  "parentCategoryId": "String",
  "platforms": "String",
  "rootCategoryId": "String",
  "settingUsage": "String",
  "technologies": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationCategory",
  "id": "d7c49ed0-9ed0-d7c4-d09e-c4d7d09ec4d7",
  "childCategoryIds": [
    "String"
  ],
  "description": "String",
  "displayName": "String",
  "helpText": "String",
  "name": "String",
  "parentCategoryId": "String",
  "platforms": "String",
  "rootCategoryId": "String",
  "settingUsage": "String",
  "technologies": "String"
}
```


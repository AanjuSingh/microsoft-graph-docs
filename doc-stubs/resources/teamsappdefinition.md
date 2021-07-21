---
title: "teamsAppDefinition resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# teamsAppDefinition resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List teamsAppDefinitions](../api/teamsappdefinition-list.md)|[teamsAppDefinition](../resources/teamsappdefinition.md) collection|Get a list of the [teamsAppDefinition](../resources/teamsappdefinition.md) objects and their properties.|
|[Create teamsAppDefinition](../api/teamsappdefinition-create.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Create a new [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[Get teamsAppDefinition](../api/teamsappdefinition-get.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Read the properties and relationships of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[Update teamsAppDefinition](../api/teamsappdefinition-update.md)|[teamsAppDefinition](../resources/teamsappdefinition.md)|Update the properties of a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[Delete teamsAppDefinition](../api/teamsappdefinition-delete.md)|None|Deletes a [teamsAppDefinition](../resources/teamsappdefinition.md) object.|
|[List teamworkBot](../api/teamsappdefinition-list-bot.md)|[teamworkBot](../resources/teamworkbot.md) collection|Get the teamworkBot resources from the bot navigation property.|
|[Create teamworkBot](../api/teamsappdefinition-post-bot.md)|[teamworkBot](../resources/teamworkbot.md)|Create a new teamworkBot object.|
|[List teamsAppIcon](../api/teamsappdefinition-list-coloricon.md)|[teamsAppIcon](../resources/teamsappicon.md) collection|Get the teamsAppIcon resources from the colorIcon navigation property.|
|[Create teamsAppIcon](../api/teamsappdefinition-post-coloricon.md)|[teamsAppIcon](../resources/teamsappicon.md)|Create a new teamsAppIcon object.|
|[List teamsAppIcon](../api/teamsappdefinition-list-outlineicon.md)|[teamsAppIcon](../resources/teamsappicon.md) collection|Get the teamsAppIcon resources from the outlineIcon navigation property.|
|[Create teamsAppIcon](../api/teamsappdefinition-post-outlineicon.md)|[teamsAppIcon](../resources/teamsappicon.md)|Create a new teamsAppIcon object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowedInstallationScopes|teamsAppInstallationScopes|**TODO: Add Description**. Possible values are: `team`, `groupChat`, `personal`, `unknownFutureValue`.|
|azureADAppId|String|**TODO: Add Description**|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|publishingState|teamsAppPublishingState|**TODO: Add Description**. Possible values are: `submitted`, `rejected`, `published`, `unknownFutureValue`.|
|shortdescription|String|**TODO: Add Description**|
|teamsAppId|String|**TODO: Add Description**|
|version|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|bot|[teamworkBot](../resources/teamworkbot.md)|**TODO: Add Description**|
|colorIcon|[teamsAppIcon](../resources/teamsappicon.md)|**TODO: Add Description**|
|outlineIcon|[teamsAppIcon](../resources/teamsappicon.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAppDefinition",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.teamsAppDefinition",
  "id": "String (identifier)",
  "allowedInstallationScopes": "String",
  "azureADAppId": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "publishingState": "String",
  "shortdescription": "String",
  "teamsAppId": "String",
  "version": "String"
}
```


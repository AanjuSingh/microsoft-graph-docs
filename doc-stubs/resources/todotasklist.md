---
title: "todoTaskList resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# todoTaskList resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List todoTaskLists](../api/todotasklist-list.md)|[todoTaskList](../resources/todotasklist.md) collection|Get a list of the [todoTaskList](../resources/todotasklist.md) objects and their properties.|
|[Create todoTaskList](../api/todotasklist-create.md)|[todoTaskList](../resources/todotasklist.md)|Create a new [todoTaskList](../resources/todotasklist.md) object.|
|[Get todoTaskList](../api/todotasklist-get.md)|[todoTaskList](../resources/todotasklist.md)|Read the properties and relationships of a [todoTaskList](../resources/todotasklist.md) object.|
|[Update todoTaskList](../api/todotasklist-update.md)|[todoTaskList](../resources/todotasklist.md)|Update the properties of a [todoTaskList](../resources/todotasklist.md) object.|
|[Delete todoTaskList](../api/todotasklist-delete.md)|None|Deletes a [todoTaskList](../resources/todotasklist.md) object.|
|[delta](../api/todotasklist-delta.md)|[todoTaskList](../resources/todotasklist.md) collection|**TODO: Add Description**|
|[List extensions](../api/todotasklist-list-extensions.md)|[extension](../resources/extension.md) collection|Get the extension resources from the extensions navigation property.|
|[Create extension](../api/todotasklist-post-extensions.md)|[extension](../resources/extension.md)|Create a new extension object.|
|[List tasks](../api/todotasklist-list-tasks.md)|[todoTask](../resources/todotask.md) collection|Get the todoTask resources from the tasks navigation property.|
|[Create todoTask](../api/todotasklist-post-tasks.md)|[todoTask](../resources/todotask.md)|Create a new todoTask object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|isOwner|Boolean|**TODO: Add Description**|
|isShared|Boolean|**TODO: Add Description**|
|wellknownListName|wellknownListName|**TODO: Add Description**. Possible values are: `none`, `defaultList`, `flaggedEmails`, `unknownFutureValue`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|extensions|[extension](../resources/extension.md) collection|**TODO: Add Description**|
|tasks|[todoTask](../resources/todotask.md) collection|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.todoTaskList",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.todoTaskList",
  "id": "String (identifier)",
  "displayName": "String",
  "isOwner": "Boolean",
  "isShared": "Boolean",
  "wellknownListName": "String"
}
```


---
title: "unifiedRoleAssignmentMultiple resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# unifiedRoleAssignmentMultiple resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List unifiedRoleAssignmentMultiples](../api/unifiedroleassignmentmultiple-list.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) collection|Get a list of the [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) objects and their properties.|
|[Create unifiedRoleAssignmentMultiple](../api/rbacapplicationmultiple-post-roleassignments.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Create a new [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[Get unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-get.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Read the properties and relationships of an [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[Update unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-update.md)|[unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md)|Update the properties of an [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[Delete unifiedRoleAssignmentMultiple](../api/unifiedroleassignmentmultiple-delete.md)|None|Deletes an [unifiedRoleAssignmentMultiple](../resources/unifiedroleassignmentmultiple.md) object.|
|[List appScopes](../api/unifiedroleassignmentmultiple-list-appscopes.md)|[appScope](../resources/appscope.md) collection|Get the appScope resources from the appScopes navigation property.|
|[Create appScope](../api/unifiedroleassignmentmultiple-post-appscopes.md)|[appScope](../resources/appscope.md)|Create a new appScope object.|
|[List directoryScopes](../api/unifiedroleassignmentmultiple-list-directoryscopes.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the directoryScopes navigation property.|
|[Add directoryScopes](../api/unifiedroleassignmentmultiple-post-directoryscopes.md)|[directoryObject](../resources/directoryobject.md)|Add directoryScopes by posting to the directoryScopes collection.|
|[List principals](../api/unifiedroleassignmentmultiple-list-principals.md)|[directoryObject](../resources/directoryobject.md) collection|Get the directoryObject resources from the principals navigation property.|
|[Add principals](../api/unifiedroleassignmentmultiple-post-principals.md)|[directoryObject](../resources/directoryobject.md)|Add principals by posting to the principals collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|appScopeIds|String collection|**TODO: Add Description**|
|condition|String|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|directoryScopeIds|String collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|principalIds|String collection|**TODO: Add Description**|
|roleDefinitionId|String|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|appScopes|[appScope](../resources/appscope.md) collection|**TODO: Add Description**|
|directoryScopes|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|principals|[directoryObject](../resources/directoryobject.md) collection|**TODO: Add Description**|
|roleDefinition|[unifiedRoleDefinition](../resources/unifiedroledefinition.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.unifiedRoleAssignmentMultiple",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unifiedRoleAssignmentMultiple",
  "id": "String (identifier)",
  "roleDefinitionId": "String",
  "condition": "String",
  "displayName": "String",
  "description": "String",
  "principalIds": [
    "String"
  ],
  "directoryScopeIds": [
    "String"
  ],
  "appScopeIds": [
    "String"
  ]
}
```


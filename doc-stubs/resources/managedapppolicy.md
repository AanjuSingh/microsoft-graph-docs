---
title: "managedAppPolicy resource type"
description: "The ManagedAppPolicy resource represents a base type for platform specific policies."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# managedAppPolicy resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

The ManagedAppPolicy resource represents a base type for platform specific policies.
This is an abstract type.


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List managedAppPolicies](../api/managedapppolicy-list.md)|[managedAppPolicy](../resources/managedapppolicy.md) collection|Get a list of the [managedAppPolicy](../resources/managedapppolicy.md) objects and their properties.|
|[Create managedAppPolicy](../api/managedapppolicy-create.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Create a new [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[Get managedAppPolicy](../api/managedapppolicy-get.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Read the properties and relationships of a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[Update managedAppPolicy](../api/managedapppolicy-update.md)|[managedAppPolicy](../resources/managedapppolicy.md)|Update the properties of a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[Delete managedAppPolicy](../api/managedapppolicy-delete.md)|None|Deletes a [managedAppPolicy](../resources/managedapppolicy.md) object.|
|[targetApps](../api/managedapppolicy-targetapps.md)|None|**TODO: Add Description**|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The date and time the policy was created.|
|description|String|The policy's description.|
|displayName|String|Policy display name.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|Last time the policy was modified.|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|version|String|Version of the entity.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "version": "String"
}
```


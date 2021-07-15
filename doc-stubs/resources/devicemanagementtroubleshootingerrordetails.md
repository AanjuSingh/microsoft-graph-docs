---
title: "deviceManagementTroubleshootingErrorDetails resource type"
description: "Object containing detailed information about the error and its remediation."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceManagementTroubleshootingErrorDetails resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Object containing detailed information about the error and its remediation.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|context|String|**TODO: Add Description**|
|failure|String|**TODO: Add Description**|
|failureDetails|String|The detailed description of what went wrong.|
|remediation|String|The detailed description of how to remediate this issue.|
|resources|[deviceManagementTroubleshootingErrorResource](../resources/devicemanagementtroubleshootingerrorresource.md) collection|Links to helpful documentation about this failure.|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingErrorDetails",
  "context": "String",
  "failure": "String",
  "failureDetails": "String",
  "remediation": "String",
  "resources": [
    {
      "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource"
    }
  ]
}
```


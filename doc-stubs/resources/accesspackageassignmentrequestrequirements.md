---
title: "accessPackageAssignmentRequestRequirements resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessPackageAssignmentRequestRequirements resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|allowCustomAssignmentSchedule|Boolean|**TODO: Add Description**|
|existingAnswers|[accessPackageAnswer](../resources/accesspackageanswer.md) collection|**TODO: Add Description**|
|isApprovalRequiredForAdd|Boolean|**TODO: Add Description**|
|isApprovalRequiredForUpdate|Boolean|**TODO: Add Description**|
|policyDescription|String|**TODO: Add Description**|
|policyDisplayName|String|**TODO: Add Description**|
|policyId|String|**TODO: Add Description**|
|questions|[accessPackageQuestion](../resources/accesspackagequestion.md) collection|**TODO: Add Description**|
|schedule|[requestSchedule](../resources/requestschedule.md)|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequestRequirements"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignmentRequestRequirements",
  "allowCustomAssignmentSchedule": "Boolean",
  "existingAnswers": [
    {
      "@odata.type": "microsoft.graph.accessPackageAnswerString"
    }
  ],
  "isApprovalRequiredForAdd": "Boolean",
  "isApprovalRequiredForUpdate": "Boolean",
  "policyDescription": "String",
  "policyDisplayName": "String",
  "policyId": "String",
  "questions": [
    {
      "@odata.type": "microsoft.graph.accessPackageMultipleChoiceQuestion"
    }
  ],
  "schedule": {
    "@odata.type": "microsoft.graph.requestSchedule"
  }
}
```


---
title: "accessReviewScheduleSettings resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# accessReviewScheduleSettings resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|applyActions|[accessReviewApplyAction](../resources/accessreviewapplyaction.md) collection|**TODO: Add Description**|
|autoApplyDecisionsEnabled|Boolean|**TODO: Add Description**|
|defaultDecision|String|**TODO: Add Description**|
|defaultDecisionEnabled|Boolean|**TODO: Add Description**|
|instanceDurationInDays|Int32|**TODO: Add Description**|
|justificationRequiredOnApproval|Boolean|**TODO: Add Description**|
|mailNotificationsEnabled|Boolean|**TODO: Add Description**|
|recommendationLookBackDuration|Duration|**TODO: Add Description**|
|recommendationsEnabled|Boolean|**TODO: Add Description**|
|recurrence|[patternedRecurrence](../resources/patternedrecurrence.md)|**TODO: Add Description**|
|reminderNotificationsEnabled|Boolean|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScheduleSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScheduleSettings",
  "applyActions": [
    {
      "@odata.type": "microsoft.graph.disableAndDeleteUserApplyAction"
    }
  ],
  "autoApplyDecisionsEnabled": "Boolean",
  "defaultDecision": "String",
  "defaultDecisionEnabled": "Boolean",
  "instanceDurationInDays": "Integer",
  "justificationRequiredOnApproval": "Boolean",
  "mailNotificationsEnabled": "Boolean",
  "recommendationLookBackDuration": "String (duration)",
  "recommendationsEnabled": "Boolean",
  "recurrence": {
    "@odata.type": "microsoft.graph.patternedRecurrence"
  },
  "reminderNotificationsEnabled": "Boolean"
}
```


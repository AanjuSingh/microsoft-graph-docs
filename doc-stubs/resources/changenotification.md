---
title: "changeNotification resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# changeNotification resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

## Properties
|Property|Type|Description|
|:---|:---|:---|
|changeType|changeType|**TODO: Add Description**. Possible values are: `created`, `updated`, `deleted`.|
|clientState|String|**TODO: Add Description**|
|encryptedContent|[changeNotificationEncryptedContent](../resources/changenotificationencryptedcontent.md)|**TODO: Add Description**|
|id|String|**TODO: Add Description**|
|lifecycleEvent|lifecycleEventType|**TODO: Add Description**. Possible values are: `missed`, `subscriptionRemoved`, `reauthorizationRequired`.|
|resource|String|**TODO: Add Description**|
|resourceData|[resourceData](../resources/resourcedata.md)|**TODO: Add Description**|
|subscriptionExpirationDateTime|DateTimeOffset|**TODO: Add Description**|
|subscriptionId|Guid|**TODO: Add Description**|
|tenantId|Guid|**TODO: Add Description**|

## Relationships
None.

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.changeNotification"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.changeNotification",
  "changeType": "String",
  "clientState": "String",
  "encryptedContent": {
    "@odata.type": "microsoft.graph.changeNotificationEncryptedContent"
  },
  "id": "String (identifier)",
  "lifecycleEvent": "String",
  "resource": "String",
  "resourceData": {
    "@odata.type": "microsoft.graph.resourceData"
  },
  "subscriptionExpirationDateTime": "String (timestamp)",
  "subscriptionId": "Guid",
  "tenantId": "Guid"
}
```


---
title: "mailAssessmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# mailAssessmentRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [threatAssessmentRequest](../resources/threatassessmentrequest.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List mailAssessmentRequests](../api/mailassessmentrequest-list.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md) collection|Get a list of the [mailAssessmentRequest](../resources/mailassessmentrequest.md) objects and their properties.|
|[Create mailAssessmentRequest](../api/mailassessmentrequest-create.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md)|Create a new [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[Get mailAssessmentRequest](../api/mailassessmentrequest-get.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md)|Read the properties and relationships of a [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[Update mailAssessmentRequest](../api/mailassessmentrequest-update.md)|[mailAssessmentRequest](../resources/mailassessmentrequest.md)|Update the properties of a [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[Delete mailAssessmentRequest](../api/mailassessmentrequest-delete.md)|None|Deletes a [mailAssessmentRequest](../resources/mailassessmentrequest.md) object.|
|[List results](../api/mailassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|Get the threatAssessmentResult resources from the results navigation property.|
|[Create threatAssessmentResult](../api/mailassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Create a new threatAssessmentResult object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|threatCategory|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentType|threatAssessmentContentType|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md).|
|destinationRoutingReason|mailDestinationRoutingReason|**TODO: Add Description**. Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`, `unknownFutureValue`.|
|expectedAssessment|threatExpectedAssessment|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `block`, `unblock`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|messageUri|String|**TODO: Add Description**|
|recipientEmail|String|**TODO: Add Description**|
|requestSource|threatAssessmentRequestSource|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `user`, `administrator`.|
|status|threatAssessmentStatus|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `pending`, `completed`.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|results|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md)|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mailAssessmentRequest",
  "baseType": "microsoft.graph.threatAssessmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mailAssessmentRequest",
  "id": "String (identifier)",
  "category": "String",
  "contentType": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "expectedAssessment": "String",
  "requestSource": "String",
  "status": "String",
  "destinationRoutingReason": "String",
  "messageUri": "String",
  "recipientEmail": "String"
}
```


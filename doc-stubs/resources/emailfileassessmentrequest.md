---
title: "emailFileAssessmentRequest resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# emailFileAssessmentRequest resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [threatAssessmentRequest](../resources/threatassessmentrequest.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List emailFileAssessmentRequests](../api/emailfileassessmentrequest-list.md)|[emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) collection|Get a list of the [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) objects and their properties.|
|[Create emailFileAssessmentRequest](../api/emailfileassessmentrequest-create.md)|[emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md)|Create a new [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[Get emailFileAssessmentRequest](../api/emailfileassessmentrequest-get.md)|[emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md)|Read the properties and relationships of an [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[Update emailFileAssessmentRequest](../api/emailfileassessmentrequest-update.md)|[emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md)|Update the properties of an [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[Delete emailFileAssessmentRequest](../api/emailfileassessmentrequest-delete.md)|None|Deletes an [emailFileAssessmentRequest](../resources/emailfileassessmentrequest.md) object.|
|[List results](../api/emailfileassessmentrequest-list-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md) collection|Get the threatAssessmentResult resources from the results navigation property.|
|[Create threatAssessmentResult](../api/emailfileassessmentrequest-post-results.md)|[threatAssessmentResult](../resources/threatassessmentresult.md)|Create a new threatAssessmentResult object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|category|threatCategory|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `undefined`, `spam`, `phishing`, `malware`, `unknownFutureValue`.|
|contentData|String|**TODO: Add Description**|
|contentType|threatAssessmentContentType|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `mail`, `url`, `file`.|
|createdBy|[identitySet](../resources/identityset.md)|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md).|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md).|
|destinationRoutingReason|mailDestinationRoutingReason|**TODO: Add Description**. Possible values are: `none`, `mailFlowRule`, `safeSender`, `blockedSender`, `advancedSpamFiltering`, `domainAllowList`, `domainBlockList`, `notInAddressBook`, `firstTimeSender`, `autoPurgeToInbox`, `autoPurgeToJunk`, `autoPurgeToDeleted`, `outbound`, `notJunk`, `junk`, `unknownFutureValue`.|
|expectedAssessment|threatExpectedAssessment|**TODO: Add Description** Inherited from [threatAssessmentRequest](../resources/threatassessmentrequest.md). Possible values are: `block`, `unblock`.|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
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
  "@odata.type": "microsoft.graph.emailFileAssessmentRequest",
  "baseType": "microsoft.graph.threatAssessmentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.emailFileAssessmentRequest",
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
  "contentData": "String",
  "destinationRoutingReason": "String",
  "recipientEmail": "String"
}
```


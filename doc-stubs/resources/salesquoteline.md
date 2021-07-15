---
title: "salesQuoteLine resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# salesQuoteLine resource type

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**


Inherits from [entity](../resources/entity.md).

## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List salesQuoteLines](../api/salesquoteline-list.md)|[salesQuoteLine](../resources/salesquoteline.md) collection|Get a list of the [salesQuoteLine](../resources/salesquoteline.md) objects and their properties.|
|[Create salesQuoteLine](../api/salesquoteline-create.md)|[salesQuoteLine](../resources/salesquoteline.md)|Create a new [salesQuoteLine](../resources/salesquoteline.md) object.|
|[Get salesQuoteLine](../api/salesquoteline-get.md)|[salesQuoteLine](../resources/salesquoteline.md)|Read the properties and relationships of a [salesQuoteLine](../resources/salesquoteline.md) object.|
|[Update salesQuoteLine](../api/salesquoteline-update.md)|[salesQuoteLine](../resources/salesquoteline.md)|Update the properties of a [salesQuoteLine](../resources/salesquoteline.md) object.|
|[Delete salesQuoteLine](../api/salesquoteline-delete.md)|None|Deletes a [salesQuoteLine](../resources/salesquoteline.md) object.|
|[List account](../api/salesquoteline-list-account.md)|[account](../resources/account.md) collection|Get the account resources from the account navigation property.|
|[Create account](../api/salesquoteline-post-account.md)|[account](../resources/account.md)|Create a new account object.|
|[List item](../api/salesquoteline-list-item.md)|[item](../resources/item.md) collection|Get the item resources from the item navigation property.|
|[Create item](../api/salesquoteline-post-item.md)|[item](../resources/item.md)|Create a new item object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|accountId|Guid|**TODO: Add Description**|
|amountExcludingTax|Decimal|**TODO: Add Description**|
|amountIncludingTax|Decimal|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|documentId|Guid|**TODO: Add Description**|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md).|
|itemId|Guid|**TODO: Add Description**|
|lineType|String|**TODO: Add Description**|
|netAmount|Decimal|**TODO: Add Description**|
|netAmountIncludingTax|Decimal|**TODO: Add Description**|
|netTaxAmount|Decimal|**TODO: Add Description**|
|quantity|Decimal|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|taxCode|String|**TODO: Add Description**|
|taxPercent|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|unitOfMeasureId|Guid|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|account|[account](../resources/account.md)|**TODO: Add Description**|
|item|[item](../resources/item.md)|**TODO: Add Description**|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.salesQuoteLine",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.salesQuoteLine",
  "id": "String (identifier)",
  "accountId": "Guid",
  "amountExcludingTax": "Decimal",
  "amountIncludingTax": "Decimal",
  "description": "String",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "discountPercent": "Decimal",
  "documentId": "Guid",
  "itemId": "Guid",
  "lineType": "String",
  "netAmount": "Decimal",
  "netAmountIncludingTax": "Decimal",
  "netTaxAmount": "Decimal",
  "quantity": "Decimal",
  "sequence": "Integer",
  "taxCode": "String",
  "taxPercent": "Decimal",
  "totalTaxAmount": "Decimal",
  "unitOfMeasureId": "Guid",
  "unitPrice": "Decimal"
}
```


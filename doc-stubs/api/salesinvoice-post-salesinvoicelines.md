---
title: "Create salesInvoiceLine"
description: "Create a new salesInvoiceLine object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create salesInvoiceLine
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new salesInvoiceLine object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [salesInvoiceLine](../resources/salesinvoiceline.md) object.

The following table shows the properties that are required when you create the [salesInvoiceLine](../resources/salesinvoiceline.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|accountId|Guid|**TODO: Add Description**|
|amountExcludingTax|Decimal|**TODO: Add Description**|
|amountIncludingTax|Decimal|**TODO: Add Description**|
|description|String|**TODO: Add Description**|
|discountAmount|Decimal|**TODO: Add Description**|
|discountAppliedBeforeTax|Boolean|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|documentId|Guid|**TODO: Add Description**|
|invoiceDiscountAllocation|Decimal|**TODO: Add Description**|
|itemId|Guid|**TODO: Add Description**|
|lineType|String|**TODO: Add Description**|
|netAmount|Decimal|**TODO: Add Description**|
|netAmountIncludingTax|Decimal|**TODO: Add Description**|
|netTaxAmount|Decimal|**TODO: Add Description**|
|quantity|Decimal|**TODO: Add Description**|
|sequence|Int32|**TODO: Add Description**|
|shipmentDate|Date|**TODO: Add Description**|
|taxCode|String|**TODO: Add Description**|
|taxPercent|Decimal|**TODO: Add Description**|
|totalTaxAmount|Decimal|**TODO: Add Description**|
|unitOfMeasureId|Guid|**TODO: Add Description**|
|unitPrice|Decimal|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [salesInvoiceLine](../resources/salesinvoiceline.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_salesinvoiceline_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/salesInvoiceLines
Content-Type: application/json
Content-length: 719

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "accountId": "Guid",
  "amountExcludingTax": "Decimal",
  "amountIncludingTax": "Decimal",
  "description": "String",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "discountPercent": "Decimal",
  "documentId": "Guid",
  "invoiceDiscountAllocation": "Decimal",
  "itemId": "Guid",
  "lineType": "String",
  "netAmount": "Decimal",
  "netAmountIncludingTax": "Decimal",
  "netTaxAmount": "Decimal",
  "quantity": "Decimal",
  "sequence": "Integer",
  "shipmentDate": "Date",
  "taxCode": "String",
  "taxPercent": "Decimal",
  "totalTaxAmount": "Decimal",
  "unitOfMeasureId": "Guid",
  "unitPrice": "Decimal"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.salesInvoiceLine"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.salesInvoiceLine",
  "id": "eddf16b5-16b5-eddf-b516-dfedb516dfed",
  "accountId": "Guid",
  "amountExcludingTax": "Decimal",
  "amountIncludingTax": "Decimal",
  "description": "String",
  "discountAmount": "Decimal",
  "discountAppliedBeforeTax": "Boolean",
  "discountPercent": "Decimal",
  "documentId": "Guid",
  "invoiceDiscountAllocation": "Decimal",
  "itemId": "Guid",
  "lineType": "String",
  "netAmount": "Decimal",
  "netAmountIncludingTax": "Decimal",
  "netTaxAmount": "Decimal",
  "quantity": "Decimal",
  "sequence": "Integer",
  "shipmentDate": "Date",
  "taxCode": "String",
  "taxPercent": "Decimal",
  "totalTaxAmount": "Decimal",
  "unitOfMeasureId": "Guid",
  "unitPrice": "Decimal"
}
```


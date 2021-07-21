---
title: "Get purchaseInvoice"
description: "Read the properties and relationships of a purchaseInvoice object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get purchaseInvoice
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [purchaseInvoice](../resources/purchaseinvoice.md) object.

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
GET /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}
```

## Optional query parameters
This method supports some of the OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a [purchaseInvoice](../resources/purchaseinvoice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_purchaseinvoice"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.purchaseInvoice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.purchaseInvoice",
    "id": "ac6993de-93de-ac69-de93-69acde9369ac",
    "buyFromAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "currencyCode": "String",
    "currencyId": "Guid",
    "discountAmount": "Decimal",
    "discountAppliedBeforeTax": "Boolean",
    "dueDate": "Date",
    "invoiceDate": "Date",
    "lastModifiedDateTime": "String (timestamp)",
    "number": "String",
    "payToAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "payToContact": "String",
    "payToName": "String",
    "payToVendorId": "Guid",
    "payToVendorNumber": "String",
    "pricesIncludeTax": "Boolean",
    "shipToAddress": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "shipToContact": "String",
    "shipToName": "String",
    "status": "String",
    "totalAmountExcludingTax": "Decimal",
    "totalAmountIncludingTax": "Decimal",
    "totalTaxAmount": "Decimal",
    "vendorId": "Guid",
    "vendorInvoiceNumber": "String",
    "vendorName": "String",
    "vendorNumber": "String"
  }
}
```


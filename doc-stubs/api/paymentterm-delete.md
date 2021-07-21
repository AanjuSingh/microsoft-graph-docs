---
title: "Delete paymentTerm"
description: "Deletes a paymentTerm object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Delete paymentTerm
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Deletes a [paymentTerm](../resources/paymentterm.md) object.

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
DELETE /financials/companies/{companyId}/paymentTerms/{paymentTermId}
DELETE /financials/companies/{companyId}/salesOrders/{salesOrderId}/paymentTerm
DELETE /financials/companies/{companyId}/salesQuotes/{salesQuoteId}/paymentTerm
DELETE /financials/companies/{companyId}/salesInvoices/{salesInvoiceId}/paymentTerm
DELETE /financials/companies/{companyId}/salesCreditMemos/{salesCreditMemoId}/paymentTerm
DELETE /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor/paymentTerm
DELETE /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}/customer/paymentTerm
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "delete_paymentterm"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/financials/companies/{companyId}/paymentTerms/{paymentTermId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```


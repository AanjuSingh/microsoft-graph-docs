---
title: "Create paymentTerm"
description: "Create a new paymentTerm object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create paymentTerm
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [paymentTerm](../resources/paymentterm.md) object.

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
POST /financials/companies/{companyId}/paymentTerms
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [paymentTerm](../resources/paymentterm.md) object.

The following table shows the properties that are required when you create the [paymentTerm](../resources/paymentterm.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|calculateDiscountOnCreditMemos|Boolean|**TODO: Add Description**|
|code|String|**TODO: Add Description**|
|discountDateCalculation|String|**TODO: Add Description**|
|discountPercent|Decimal|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|dueDateCalculation|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [paymentTerm](../resources/paymentterm.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_paymentterm_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/financials/companies/{companyId}/paymentTerms
Content-Type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.paymentTerm",
  "calculateDiscountOnCreditMemos": "Boolean",
  "code": "String",
  "discountDateCalculation": "String",
  "discountPercent": "Decimal",
  "displayName": "String",
  "dueDateCalculation": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.paymentTerm"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.paymentTerm",
  "id": "06f25a64-5a64-06f2-645a-f206645af206",
  "calculateDiscountOnCreditMemos": "Boolean",
  "code": "String",
  "discountDateCalculation": "String",
  "discountPercent": "Decimal",
  "displayName": "String",
  "dueDateCalculation": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```


---
title: "Update picture"
description: "Update the properties of a picture object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update picture
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [picture](../resources/picture.md) object.

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
PATCH /financials/companies/{companyId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/items/{itemId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/employees/{employeeId}/picture/{pictureId}
PATCH /financials/companies/{companyId}/purchaseInvoices/{purchaseInvoiceId}/vendor/picture/{pictureId}
PATCH /financials/companies/{companyId}/customerPaymentJournals/{customerPaymentJournalId}/customerPayments/{customerPaymentId}/customer/picture/{pictureId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [picture](../resources/picture.md) object.

The following table shows the properties that are required when you update the [picture](../resources/picture.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|Stream|**TODO: Add Description**|
|contentType|String|**TODO: Add Description**|
|height|Int32|**TODO: Add Description**|
|width|Int32|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [picture](../resources/picture.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_picture"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/financials/companies/{companyId}/picture/{pictureId}
Content-Type: application/json
Content-length: 148

{
  "@odata.type": "#microsoft.graph.picture",
  "content": "Stream",
  "contentType": "String",
  "height": "Integer",
  "width": "Integer"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.picture",
  "id": "8c785410-5410-8c78-1054-788c1054788c",
  "content": "Stream",
  "contentType": "String",
  "height": "Integer",
  "width": "Integer"
}
```


---
title: "Update bookingCurrency"
description: "Update the properties of a bookingCurrency object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update bookingCurrency
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [bookingCurrency](../resources/bookingcurrency.md) object.

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
PATCH /bookingCurrencies/{bookingCurrenciesId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [bookingCurrency](../resources/bookingcurrency.md) object.

The following table shows the properties that are required when you update the [bookingCurrency](../resources/bookingcurrency.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|symbol|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [bookingCurrency](../resources/bookingcurrency.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_bookingcurrency"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/bookingCurrencies/{bookingCurrenciesId}
Content-Type: application/json
Content-length: 80

{
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "symbol": "String"
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
  "@odata.type": "#microsoft.graph.bookingCurrency",
  "id": "aa75bf0d-bf0d-aa75-0dbf-75aa0dbf75aa",
  "symbol": "String"
}
```


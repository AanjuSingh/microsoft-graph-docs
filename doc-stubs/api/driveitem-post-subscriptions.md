---
title: "Create subscription"
description: "Create a new subscription object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create subscription
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new subscription object.

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
POST /workbooks/{workbooksId}/subscriptions
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [subscription](../resources/subscription.md) object.

The following table shows the properties that are required when you create the [subscription](../resources/subscription.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|applicationId|String|**TODO: Add Description**|
|changeType|String|**TODO: Add Description**|
|clientState|String|**TODO: Add Description**|
|creatorId|String|**TODO: Add Description**|
|encryptionCertificate|String|**TODO: Add Description**|
|encryptionCertificateId|String|**TODO: Add Description**|
|expirationDateTime|DateTimeOffset|**TODO: Add Description**|
|includeResourceData|Boolean|**TODO: Add Description**|
|latestSupportedTlsVersion|String|**TODO: Add Description**|
|lifecycleNotificationUrl|String|**TODO: Add Description**|
|notificationContentType|String|**TODO: Add Description**|
|notificationQueryOptions|String|**TODO: Add Description**|
|notificationUrl|String|**TODO: Add Description**|
|resource|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [subscription](../resources/subscription.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_subscription_from_subscriptions"
}
-->
``` http
POST https://graph.microsoft.com/beta/workbooks/{workbooksId}/subscriptions
Content-Type: application/json
Content-length: 548

{
  "@odata.type": "#microsoft.graph.subscription",
  "applicationId": "String",
  "changeType": "String",
  "clientState": "String",
  "creatorId": "String",
  "encryptionCertificate": "String",
  "encryptionCertificateId": "String",
  "expirationDateTime": "String (timestamp)",
  "includeResourceData": "Boolean",
  "latestSupportedTlsVersion": "String",
  "lifecycleNotificationUrl": "String",
  "notificationContentType": "String",
  "notificationQueryOptions": "String",
  "notificationUrl": "String",
  "resource": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.subscription",
  "id": "0f562fc8-2fc8-0f56-c82f-560fc82f560f",
  "applicationId": "String",
  "changeType": "String",
  "clientState": "String",
  "creatorId": "String",
  "encryptionCertificate": "String",
  "encryptionCertificateId": "String",
  "expirationDateTime": "String (timestamp)",
  "includeResourceData": "Boolean",
  "latestSupportedTlsVersion": "String",
  "lifecycleNotificationUrl": "String",
  "notificationContentType": "String",
  "notificationQueryOptions": "String",
  "notificationUrl": "String",
  "resource": "String"
}
```


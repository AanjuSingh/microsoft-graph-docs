---
title: "Update dataSharingConsent"
description: "Update the properties of a dataSharingConsent object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update dataSharingConsent
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [dataSharingConsent](../resources/datasharingconsent.md) object.

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
PATCH /deviceManagement/dataSharingConsents/{dataSharingConsentId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [dataSharingConsent](../resources/datasharingconsent.md) object.

The following table shows the properties that are required when you update the [dataSharingConsent](../resources/datasharingconsent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|grantDateTime|DateTimeOffset|The time consent was granted for this account|
|granted|Boolean|The granted state for the data sharing consent|
|grantedByUpn|String|The Upn of the user that granted consent for this account|
|grantedByUserId|String|The UserId of the user that granted consent for this account|
|serviceDisplayName|String|The display name of the service work flow|
|termsUrl|String|The TermsUrl for the data sharing consent|



## Response

If successful, this method returns a `200 OK` response code and an updated [dataSharingConsent](../resources/datasharingconsent.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_datasharingconsent"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/dataSharingConsents/{dataSharingConsentId}
Content-Type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "grantDateTime": "String (timestamp)",
  "granted": "Boolean",
  "grantedByUpn": "String",
  "grantedByUserId": "String",
  "serviceDisplayName": "String",
  "termsUrl": "String"
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
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "0cac5df4-5df4-0cac-f45d-ac0cf45dac0c",
  "grantDateTime": "String (timestamp)",
  "granted": "Boolean",
  "grantedByUpn": "String",
  "grantedByUserId": "String",
  "serviceDisplayName": "String",
  "termsUrl": "String"
}
```


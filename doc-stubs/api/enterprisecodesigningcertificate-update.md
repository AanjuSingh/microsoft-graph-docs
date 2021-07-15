---
title: "Update enterpriseCodeSigningCertificate"
description: "Update the properties of an enterpriseCodeSigningCertificate object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update enterpriseCodeSigningCertificate
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.

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
PATCH /deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object.

The following table shows the properties that are required when you update the [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|content|Binary|The Windows Enterprise Code-Signing Certificate in the raw data format.|
|expirationDateTime|DateTimeOffset|The Cert Expiration Date.|
|issuer|String|The Issuer value for the cert.|
|issuerName|String|The Issuer Name for the cert.|
|status|certificateStatus|The Certificate Status Provisioned or not Provisioned. Possible values are: `notProvisioned`, `provisioned`.|
|subject|String|The Subject Value for the cert.|
|subjectName|String|The Subject Name for the cert.|
|uploadDateTime|DateTimeOffset|The date time of CodeSigning Cert when it is uploaded.|



## Response

If successful, this method returns a `200 OK` response code and an updated [enterpriseCodeSigningCertificate](../resources/enterprisecodesigningcertificate.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_enterprisecodesigningcertificate"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/enterpriseCodeSigningCertificates/{enterpriseCodeSigningCertificateId}
Content-Type: application/json
Content-length: 313

{
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "content": "Binary",
  "expirationDateTime": "String (timestamp)",
  "issuer": "String",
  "issuerName": "String",
  "status": "String",
  "subject": "String",
  "subjectName": "String",
  "uploadDateTime": "String (timestamp)"
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
  "@odata.type": "#microsoft.graph.enterpriseCodeSigningCertificate",
  "id": "552cac6c-ac6c-552c-6cac-2c556cac2c55",
  "content": "Binary",
  "expirationDateTime": "String (timestamp)",
  "issuer": "String",
  "issuerName": "String",
  "status": "String",
  "subject": "String",
  "subjectName": "String",
  "uploadDateTime": "String (timestamp)"
}
```


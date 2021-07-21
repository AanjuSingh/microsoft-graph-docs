---
title: "Update androidForWorkEnrollmentProfile"
description: "Update the properties of an androidForWorkEnrollmentProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update androidForWorkEnrollmentProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.

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
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object.

The following table shows the properties that are required when you update the [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|accountId|String|Tenant GUID the enrollment profile belongs to.|
|createdDateTime|DateTimeOffset|Date time the enrollment profile was created.|
|description|String|Description for the enrollment profile.|
|displayName|String|Display name for the enrollment profile.|
|enrolledDeviceCount|Int32|Total number of Android devices that have enrolled using this enrollment profile.|
|lastModifiedDateTime|DateTimeOffset|Date time the enrollment profile was last modified.|
|qrCodeContent|String|String used to generate a QR code for the token.|
|qrCodeImage|[mimeContent](../resources/mimecontent.md)|String used to generate a QR code for the token.|
|tokenExpirationDateTime|DateTimeOffset|Date time the most recently created token will expire.|
|tokenValue|String|Value of the most recently created token for this enrollment profile.|



## Response

If successful, this method returns a `200 OK` response code and an updated [androidForWorkEnrollmentProfile](../resources/androidforworkenrollmentprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_androidforworkenrollmentprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-Type: application/json
Content-length: 377

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "String",
  "description": "String",
  "displayName": "String",
  "enrolledDeviceCount": "Integer",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "tokenExpirationDateTime": "String (timestamp)",
  "tokenValue": "String"
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
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "id": "2bd0d592-d592-2bd0-92d5-d02b92d5d02b",
  "accountId": "String",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "enrolledDeviceCount": "Integer",
  "lastModifiedDateTime": "String (timestamp)",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent"
  },
  "tokenExpirationDateTime": "String (timestamp)",
  "tokenValue": "String"
}
```


---
title: "Get importedAppleDeviceIdentityResult"
description: "Read the properties and relationships of an importedAppleDeviceIdentityResult object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get importedAppleDeviceIdentityResult
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object.

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
GET /importedAppleDeviceIdentityResult
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

If successful, this method returns a `200 OK` response code and an [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_importedappledeviceidentityresult"
}
-->
``` http
GET https://graph.microsoft.com/beta/importedAppleDeviceIdentityResult
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.importedAppleDeviceIdentityResult"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
    "id": "ddb431e8-31e8-ddb4-e831-b4dde831b4dd",
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "discoverySource": "String",
    "enrollmentState": "String",
    "isDeleted": "Boolean",
    "isSupervised": "Boolean",
    "lastContactedDateTime": "String (timestamp)",
    "platform": "String",
    "requestedEnrollmentProfileAssignmentDateTime": "String (timestamp)",
    "requestedEnrollmentProfileId": "String",
    "serialNumber": "String",
    "status": "Boolean"
  }
}
```


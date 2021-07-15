---
title: "importedAppleDeviceIdentity: importAppleDeviceIdentityList"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# importedAppleDeviceIdentity: importAppleDeviceIdentityList
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**TODO: Add Description**

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
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply JSON representation of the parameters.

The following table shows the parameters that can be used with this action.

|Parameter|Type|Description|
|:---|:---|:---|
|importedAppleDeviceIdentities|[importedAppleDeviceIdentity](../resources/importedappledeviceidentity.md) collection|**TODO: Add Description**|
|overwriteImportedDeviceIdentities|Boolean|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [importedAppleDeviceIdentityResult](../resources/importedappledeviceidentityresult.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "importedappledeviceidentity_importappledeviceidentitylist"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/importedAppleDeviceIdentities/importAppleDeviceIdentityList
Content-Type: application/json
Content-length: 676

{
  "importedAppleDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentity",
      "id": "String (identifier)",
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
      "serialNumber": "String"
    }
  ],
  "overwriteImportedDeviceIdentities": "Boolean"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.importedAppleDeviceIdentityResult)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedAppleDeviceIdentityResult",
      "id": "String (identifier)",
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
  ]
}
```


---
title: "Update importedDeviceIdentity"
description: "Update the properties of an importedDeviceIdentity object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update importedDeviceIdentity
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.

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
PATCH /deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [importedDeviceIdentity](../resources/importeddeviceidentity.md) object.

The following table shows the properties that are required when you update the [importedDeviceIdentity](../resources/importeddeviceidentity.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|Created Date Time of the device|
|description|String|The description of the device|
|enrollmentState|enrollmentState|The state of the device in Intune. Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|importedDeviceIdentifier|String|Imported Device Identifier|
|importedDeviceIdentityType|importedDeviceIdentityType|Type of Imported Device Identity. Possible values are: `unknown`, `imei`, `serialNumber`.|
|lastContactedDateTime|DateTimeOffset|Last Contacted Date Time of the device|
|lastModifiedDateTime|DateTimeOffset|Last Modified DateTime of the description|
|platform|platform|The platform of the Device. Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [importedDeviceIdentity](../resources/importeddeviceidentity.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_importeddeviceidentity"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedDeviceIdentities/{importedDeviceIdentityId}
Content-Type: application/json
Content-length: 283

{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "description": "String",
  "enrollmentState": "String",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "String (timestamp)",
  "platform": "String"
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
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "61ce6aa4-6aa4-61ce-a46a-ce61a46ace61",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastContactedDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "platform": "String"
}
```


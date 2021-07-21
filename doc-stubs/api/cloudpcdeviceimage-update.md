---
title: "Update cloudPcDeviceImage"
description: "Update the properties of a cloudPcDeviceImage object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update cloudPcDeviceImage
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.

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
PATCH /deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object.

The following table shows the properties that are required when you update the [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|**TODO: Add Description**|
|lastModifiedDateTime|DateTimeOffset|**TODO: Add Description**|
|operatingSystem|String|**TODO: Add Description**|
|osBuildNumber|String|**TODO: Add Description**|
|sourceImageResourceId|String|**TODO: Add Description**|
|status|cloudPcDeviceImageStatus|**TODO: Add Description**. Possible values are: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|**TODO: Add Description**. Possible values are: `internalServerError`, `sourceImageNotFound`, `osVersionNotSupported`, `sourceImageInvalid`.|
|version|String|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_cloudpcdeviceimage"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/deviceImages/{cloudPcDeviceImageId}
Content-Type: application/json
Content-length: 265

{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "sourceImageResourceId": "String",
  "status": "String",
  "statusDetails": "String",
  "version": "String"
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
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "6205b3c3-b3c3-6205-c3b3-0562c3b30562",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "sourceImageResourceId": "String",
  "status": "String",
  "statusDetails": "String",
  "version": "String"
}
```


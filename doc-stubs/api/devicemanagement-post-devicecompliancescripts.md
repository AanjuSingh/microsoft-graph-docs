---
title: "Create deviceComplianceScript"
description: "Create a new deviceComplianceScript object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create deviceComplianceScript
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new deviceComplianceScript object.

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
POST /deviceManagement/deviceComplianceScripts
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceComplianceScript](../resources/devicecompliancescript.md) object.

The following table shows the properties that are required when you create the [deviceComplianceScript](../resources/devicecompliancescript.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|createdDateTime|DateTimeOffset|The timestamp of when the device compliance script was created. This property is read-only.|
|description|String|Description of the device compliance script|
|detectionScriptContent|Binary|The entire content of the detection powershell script|
|displayName|String|Name of the device compliance script|
|enforceSignatureCheck|Boolean|Indicate whether the script signature needs be checked|
|lastModifiedDateTime|DateTimeOffset|The timestamp of when the device compliance script was modified. This property is read-only.|
|publisher|String|Name of the device compliance script publisher|
|roleScopeTagIds|String collection|List of Scope Tag IDs for the device compliance script|
|runAs32Bit|Boolean|Indicate whether PowerShell script(s) should run as 32-bit|
|runAsAccount|runAsAccountType|Indicates the type of execution context. Possible values are: `system`, `user`.|
|version|String|Version of the device compliance script|



## Response

If successful, this method returns a `201 Created` response code and a [deviceComplianceScript](../resources/devicecompliancescript.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_devicecompliancescript_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceComplianceScripts
Content-Type: application/json
Content-length: 349

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "description": "String",
  "detectionScriptContent": "Binary",
  "displayName": "String",
  "enforceSignatureCheck": "Boolean",
  "publisher": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": "Boolean",
  "runAsAccount": "String",
  "version": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.deviceComplianceScript"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.deviceComplianceScript",
  "id": "c387dc87-dc87-c387-87dc-87c387dc87c3",
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "detectionScriptContent": "Binary",
  "displayName": "String",
  "enforceSignatureCheck": "Boolean",
  "lastModifiedDateTime": "String (timestamp)",
  "publisher": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "runAs32Bit": "Boolean",
  "runAsAccount": "String",
  "version": "String"
}
```


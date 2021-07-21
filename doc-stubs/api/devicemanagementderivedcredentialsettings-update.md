---
title: "Update deviceManagementDerivedCredentialSettings"
description: "Update the properties of a deviceManagementDerivedCredentialSettings object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceManagementDerivedCredentialSettings
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.

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
PATCH /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object.

The following table shows the properties that are required when you update the [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|displayName|String|The display name for the profile.|
|helpUrl|String|The URL that will be accessible to end users as they retrieve a derived credential using the Company Portal.|
|issuer|deviceManagementDerivedCredentialIssuer|The derived credential provider to use. Possible values are: `intercede`, `entrustDatacard`, `purebred`, `xTec`.|
|notificationType|deviceManagementDerivedCredentialNotificationType|The methods used to inform the end user to open Company Portal to deliver Wi-Fi, VPN, or email profiles that use certificates to the device. Possible values are: `none`, `companyPortal`, `email`.|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceManagementDerivedCredentialSettings](../resources/devicemanagementderivedcredentialsettings.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementderivedcredentialsettings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
Content-Type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "displayName": "String",
  "helpUrl": "String",
  "issuer": "String",
  "notificationType": "String"
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
  "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
  "id": "0aa131c7-31c7-0aa1-c731-a10ac731a10a",
  "displayName": "String",
  "helpUrl": "String",
  "issuer": "String",
  "notificationType": "String"
}
```


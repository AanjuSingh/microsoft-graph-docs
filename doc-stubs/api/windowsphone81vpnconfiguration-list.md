---
title: "List windowsPhone81VpnConfiguration"
description: "Get a list of the windowsPhone81VpnConfiguration objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List windowsPhone81VpnConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [windowsPhone81VpnConfiguration](../resources/windowsphone81vpnconfiguration.md) objects and their properties.

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
GET ** Collection URI for microsoft.graph.windowsPhone81VpnConfiguration not found
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

If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81VpnConfiguration](../resources/windowsphone81vpnconfiguration.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_windowsphone81vpnconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Collection URI for microsoft.graph.windowsPhone81VpnConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.windowsPhone81VpnConfiguration)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81VpnConfiguration",
      "id": "a6daafd0-afd0-a6da-d0af-daa6d0afdaa6",
      "createdDateTime": "String (timestamp)",
      "description": "String",
      "deviceManagementApplicabilityRuleDeviceMode": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode"
      },
      "deviceManagementApplicabilityRuleOsEdition": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition"
      },
      "deviceManagementApplicabilityRuleOsVersion": {
        "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion"
      },
      "displayName": "String",
      "lastModifiedDateTime": "String (timestamp)",
      "roleScopeTagIds": [
        "String"
      ],
      "supportsScopeTags": "Boolean",
      "version": "Integer",
      "connectionName": "String",
      "customXml": "Binary",
      "servers": [
        {
          "@odata.type": "microsoft.graph.vpnServer"
        }
      ],
      "applyOnlyToWindows81": "Boolean",
      "connectionType": "String",
      "enableSplitTunneling": "Boolean",
      "loginGroupOrDomain": "String",
      "proxyServer": {
        "@odata.type": "microsoft.graph.windows81VpnProxyServer"
      },
      "authenticationMethod": "String",
      "bypassVpnOnCompanyWifi": "Boolean",
      "bypassVpnOnHomeWifi": "Boolean",
      "dnsSuffixSearchList": [
        "String"
      ],
      "rememberUserCredentials": "Boolean"
    }
  ]
}
```


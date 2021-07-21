---
title: "Update microsoftTunnelConfiguration"
description: "Update the properties of a microsoftTunnelConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update microsoftTunnelConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [microsoftTunnelConfiguration](../resources/microsofttunnelconfiguration.md) object.

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
PATCH /deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [microsoftTunnelConfiguration](../resources/microsofttunnelconfiguration.md) object.

The following table shows the properties that are required when you update the [microsoftTunnelConfiguration](../resources/microsofttunnelconfiguration.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|advancedSettings|[keyValuePair](../resources/keyvaluepair.md) collection|Additional settings that may be applied to the server|
|defaultDomainSuffix|String|The Default Domain appendix that will be used by the clients|
|description|String|The MicrosoftTunnelConfiguration's description|
|displayName|String|The MicrosoftTunnelConfiguration's display name|
|dnsServers|String collection|The DNS servers that will be used by the clients|
|lastUpdateDateTime|DateTimeOffset|When the MicrosoftTunnelConfiguration was last updated|
|listenPort|Int32|The port that both TCP and UPD will listen over on the server|
|network|String|The subnet that will be used to allocate virtual address for the clients|
|roleScopeTagIds|String collection|List of Scope Tags for this Entity instance.|
|routesExclude|String collection|Subsets of the routes that will not be routed by the server|
|routesInclude|String collection|The routs that will be routed by the server|
|splitDNS|String collection|The domains that will be resolved using the provided dns servers|



## Response

If successful, this method returns a `200 OK` response code and an updated [microsoftTunnelConfiguration](../resources/microsofttunnelconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_microsofttunnelconfiguration"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/microsoftTunnelConfigurations/{microsoftTunnelConfigurationId}
Content-Type: application/json
Content-length: 563

{
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "defaultDomainSuffix": "String",
  "description": "String",
  "displayName": "String",
  "dnsServers": [
    "String"
  ],
  "lastUpdateDateTime": "String (timestamp)",
  "listenPort": "Integer",
  "network": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "routesExclude": [
    "String"
  ],
  "routesInclude": [
    "String"
  ],
  "splitDNS": [
    "String"
  ]
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
  "@odata.type": "#microsoft.graph.microsoftTunnelConfiguration",
  "id": "50ee47e5-47e5-50ee-e547-ee50e547ee50",
  "advancedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "defaultDomainSuffix": "String",
  "description": "String",
  "displayName": "String",
  "dnsServers": [
    "String"
  ],
  "lastUpdateDateTime": "String (timestamp)",
  "listenPort": "Integer",
  "network": "String",
  "roleScopeTagIds": [
    "String"
  ],
  "routesExclude": [
    "String"
  ],
  "routesInclude": [
    "String"
  ],
  "splitDNS": [
    "String"
  ]
}
```


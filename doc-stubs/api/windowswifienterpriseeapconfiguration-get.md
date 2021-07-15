---
title: "Get windowsWifiEnterpriseEAPConfiguration"
description: "Read the properties and relationships of a windowsWifiEnterpriseEAPConfiguration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get windowsWifiEnterpriseEAPConfiguration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) object.

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
GET ** Entity URI for microsoft.graph.windowsWifiEnterpriseEAPConfiguration not found
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

If successful, this method returns a `200 OK` response code and a [windowsWifiEnterpriseEAPConfiguration](../resources/windowswifienterpriseeapconfiguration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_windowswifienterpriseeapconfiguration"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.windowsWifiEnterpriseEAPConfiguration not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.windowsWifiEnterpriseEAPConfiguration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsWifiEnterpriseEAPConfiguration",
    "id": "1c9c580f-580f-1c9c-0f58-9c1c0f589c1c",
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
    "connectAutomatically": "Boolean",
    "connectToPreferredNetwork": "Boolean",
    "connectWhenNetworkNameIsHidden": "Boolean",
    "forceFIPSCompliance": "Boolean",
    "meteredConnectionLimit": "String",
    "networkName": "String",
    "preSharedKey": "String",
    "proxyAutomaticConfigurationUrl": "String",
    "proxyManualAddress": "String",
    "proxyManualPort": "Integer",
    "proxySetting": "String",
    "ssid": "String",
    "wifiSecurityType": "String",
    "authenticationMethod": "String",
    "authenticationPeriodInSeconds": "Integer",
    "authenticationRetryDelayPeriodInSeconds": "Integer",
    "authenticationType": "String",
    "cacheCredentials": "Boolean",
    "disableUserPromptForServerValidation": "Boolean",
    "eapolStartPeriodInSeconds": "Integer",
    "eapType": "String",
    "enablePairwiseMasterKeyCaching": "Boolean",
    "enablePreAuthentication": "Boolean",
    "innerAuthenticationProtocolForEAPTTLS": "String",
    "maximumAuthenticationFailures": "Integer",
    "maximumAuthenticationTimeoutInSeconds": "Integer",
    "maximumEAPOLStartMessages": "Integer",
    "maximumNumberOfPairwiseMasterKeysInCache": "Integer",
    "maximumPairwiseMasterKeyCacheTimeInMinutes": "Integer",
    "maximumPreAuthenticationAttempts": "Integer",
    "networkSingleSignOn": "String",
    "outerIdentityPrivacyTemporaryValue": "String",
    "performServerValidation": "Boolean",
    "promptForAdditionalAuthenticationCredentials": "Boolean",
    "requireCryptographicBinding": "Boolean",
    "trustedServerCertificateNames": [
      "String"
    ],
    "userBasedVirtualLan": "Boolean"
  }
}
```


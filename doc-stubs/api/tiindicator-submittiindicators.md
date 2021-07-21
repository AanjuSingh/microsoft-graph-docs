---
title: "tiIndicator: submitTiIndicators"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# tiIndicator: submitTiIndicators
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
POST /security/tiIndicators/submitTiIndicators
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
|value|[tiIndicator](../resources/tiindicator.md) collection|**TODO: Add Description**|



## Response

If successful, this action returns a `200 OK` response code and a [tiIndicator](../resources/tiindicator.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "tiindicator_submittiindicators"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/tiIndicators/submitTiIndicators
Content-Type: application/json
Content-length: 2299

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "String (identifier)",
      "action": "String",
      "activityGroupNames": [
        "String"
      ],
      "additionalInformation": "String",
      "azureTenantId": "String",
      "confidence": "Integer",
      "description": "String",
      "diamondModel": "String",
      "domainName": "String",
      "emailEncoding": "String",
      "emailLanguage": "String",
      "emailRecipient": "String",
      "emailSenderAddress": "String",
      "emailSenderName": "String",
      "emailSourceDomain": "String",
      "emailSourceIpAddress": "String",
      "emailSubject": "String",
      "emailXMailer": "String",
      "expirationDateTime": "String (timestamp)",
      "externalId": "String",
      "fileCompileDateTime": "String (timestamp)",
      "fileCreatedDateTime": "String (timestamp)",
      "fileHashType": "String",
      "fileHashValue": "String",
      "fileMutexName": "String",
      "fileName": "String",
      "filePacker": "String",
      "filePath": "String",
      "fileSize": "Integer",
      "fileType": "String",
      "ingestedDateTime": "String (timestamp)",
      "isActive": "Boolean",
      "killChain": [
        "String"
      ],
      "knownFalsePositives": "String",
      "lastReportedDateTime": "String (timestamp)",
      "malwareFamilyNames": [
        "String"
      ],
      "networkCidrBlock": "String",
      "networkDestinationAsn": "Integer",
      "networkDestinationCidrBlock": "String",
      "networkDestinationIPv4": "String",
      "networkDestinationIPv6": "String",
      "networkDestinationPort": "Integer",
      "networkIPv4": "String",
      "networkIPv6": "String",
      "networkPort": "Integer",
      "networkProtocol": "Integer",
      "networkSourceAsn": "Integer",
      "networkSourceCidrBlock": "String",
      "networkSourceIPv4": "String",
      "networkSourceIPv6": "String",
      "networkSourcePort": "Integer",
      "passiveOnly": "Boolean",
      "severity": "Integer",
      "tags": [
        "String"
      ],
      "targetProduct": "String",
      "threatType": "String",
      "tlpLevel": "String",
      "url": "String",
      "userAgent": "String"
    }
  ]
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.tiIndicator)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.tiIndicator",
      "id": "String (identifier)",
      "action": "String",
      "activityGroupNames": [
        "String"
      ],
      "additionalInformation": "String",
      "azureTenantId": "String",
      "confidence": "Integer",
      "description": "String",
      "diamondModel": "String",
      "domainName": "String",
      "emailEncoding": "String",
      "emailLanguage": "String",
      "emailRecipient": "String",
      "emailSenderAddress": "String",
      "emailSenderName": "String",
      "emailSourceDomain": "String",
      "emailSourceIpAddress": "String",
      "emailSubject": "String",
      "emailXMailer": "String",
      "expirationDateTime": "String (timestamp)",
      "externalId": "String",
      "fileCompileDateTime": "String (timestamp)",
      "fileCreatedDateTime": "String (timestamp)",
      "fileHashType": "String",
      "fileHashValue": "String",
      "fileMutexName": "String",
      "fileName": "String",
      "filePacker": "String",
      "filePath": "String",
      "fileSize": "Integer",
      "fileType": "String",
      "ingestedDateTime": "String (timestamp)",
      "isActive": "Boolean",
      "killChain": [
        "String"
      ],
      "knownFalsePositives": "String",
      "lastReportedDateTime": "String (timestamp)",
      "malwareFamilyNames": [
        "String"
      ],
      "networkCidrBlock": "String",
      "networkDestinationAsn": "Integer",
      "networkDestinationCidrBlock": "String",
      "networkDestinationIPv4": "String",
      "networkDestinationIPv6": "String",
      "networkDestinationPort": "Integer",
      "networkIPv4": "String",
      "networkIPv6": "String",
      "networkPort": "Integer",
      "networkProtocol": "Integer",
      "networkSourceAsn": "Integer",
      "networkSourceCidrBlock": "String",
      "networkSourceIPv4": "String",
      "networkSourceIPv6": "String",
      "networkSourcePort": "Integer",
      "passiveOnly": "Boolean",
      "severity": "Integer",
      "tags": [
        "String"
      ],
      "targetProduct": "String",
      "threatType": "String",
      "tlpLevel": "String",
      "url": "String",
      "userAgent": "String"
    }
  ]
}
```


---
title: "Get hostSecurityProfile"
description: "Read the properties and relationships of a hostSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get hostSecurityProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [hostSecurityProfile](../resources/hostsecurityprofile.md) object.

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
GET /security/hostSecurityProfiles/{hostSecurityProfileId}
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

If successful, this method returns a `200 OK` response code and a [hostSecurityProfile](../resources/hostsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_hostsecurityprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/hostSecurityProfiles/{hostSecurityProfileId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.hostSecurityProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.hostSecurityProfile",
    "id": "4e21d592-d592-4e21-92d5-214e92d5214e",
    "azureSubscriptionId": "String",
    "azureTenantId": "String",
    "firstSeenDateTime": "String (timestamp)",
    "fqdn": "String",
    "isAzureAdJoined": "Boolean",
    "isAzureAdRegistered": "Boolean",
    "isHybridAzureDomainJoined": "Boolean",
    "lastSeenDateTime": "String (timestamp)",
    "logonUsers": [
      {
        "@odata.type": "microsoft.graph.logonUser"
      }
    ],
    "netBiosName": "String",
    "networkInterfaces": [
      {
        "@odata.type": "microsoft.graph.networkInterface"
      }
    ],
    "os": "String",
    "osVersion": "String",
    "parentHost": "String",
    "relatedHostIds": [
      "String"
    ],
    "riskScore": "String",
    "tags": [
      "String"
    ],
    "vendorInformation": {
      "@odata.type": "microsoft.graph.securityVendorInformation"
    }
  }
}
```


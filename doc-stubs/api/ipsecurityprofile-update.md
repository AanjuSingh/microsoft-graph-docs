---
title: "Update ipSecurityProfile"
description: "Update the properties of an ipSecurityProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update ipSecurityProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of an [ipSecurityProfile](../resources/ipsecurityprofile.md) object.

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
PATCH /security/ipSecurityProfiles/{ipSecurityProfileId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [ipSecurityProfile](../resources/ipsecurityprofile.md) object.

The following table shows the properties that are required when you update the [ipSecurityProfile](../resources/ipsecurityprofile.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|activityGroupNames|String collection|**TODO: Add Description**|
|address|String|**TODO: Add Description**|
|azureSubscriptionId|String|**TODO: Add Description**|
|azureTenantId|String|**TODO: Add Description**|
|countHits|Int32|**TODO: Add Description**|
|countHosts|Int32|**TODO: Add Description**|
|firstSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|ipCategories|[ipCategory](../resources/ipcategory.md) collection|**TODO: Add Description**|
|ipReferenceData|[ipReferenceData](../resources/ipreferencedata.md) collection|**TODO: Add Description**|
|lastSeenDateTime|DateTimeOffset|**TODO: Add Description**|
|riskScore|String|**TODO: Add Description**|
|tags|String collection|**TODO: Add Description**|
|vendorInformation|[securityVendorInformation](../resources/securityvendorinformation.md)|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [ipSecurityProfile](../resources/ipsecurityprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_ipsecurityprofile"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/security/ipSecurityProfiles/{ipSecurityProfileId}
Content-Type: application/json
Content-length: 689

{
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "activityGroupNames": [
    "String"
  ],
  "address": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "countHits": "Integer",
  "countHosts": "Integer",
  "firstSeenDateTime": "String (timestamp)",
  "ipCategories": [
    {
      "@odata.type": "microsoft.graph.ipCategory"
    }
  ],
  "ipReferenceData": [
    {
      "@odata.type": "microsoft.graph.ipReferenceData"
    }
  ],
  "lastSeenDateTime": "String (timestamp)",
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
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
  "@odata.type": "#microsoft.graph.ipSecurityProfile",
  "id": "8c96b1ec-b1ec-8c96-ecb1-968cecb1968c",
  "activityGroupNames": [
    "String"
  ],
  "address": "String",
  "azureSubscriptionId": "String",
  "azureTenantId": "String",
  "countHits": "Integer",
  "countHosts": "Integer",
  "firstSeenDateTime": "String (timestamp)",
  "ipCategories": [
    {
      "@odata.type": "microsoft.graph.ipCategory"
    }
  ],
  "ipReferenceData": [
    {
      "@odata.type": "microsoft.graph.ipReferenceData"
    }
  ],
  "lastSeenDateTime": "String (timestamp)",
  "riskScore": "String",
  "tags": [
    "String"
  ],
  "vendorInformation": {
    "@odata.type": "microsoft.graph.securityVendorInformation"
  }
}
```


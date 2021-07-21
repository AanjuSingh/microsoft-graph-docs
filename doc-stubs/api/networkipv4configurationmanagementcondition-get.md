---
title: "Get networkIPv4ConfigurationManagementCondition"
description: "Read the properties and relationships of a networkIPv4ConfigurationManagementCondition object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get networkIPv4ConfigurationManagementCondition
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) object.

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
GET ** Entity URI for microsoft.graph.networkIPv4ConfigurationManagementCondition not found
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

If successful, this method returns a `200 OK` response code and a [networkIPv4ConfigurationManagementCondition](../resources/networkipv4configurationmanagementcondition.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_networkipv4configurationmanagementcondition"
}
-->
``` http
GET https://graph.microsoft.com/beta** Entity URI for microsoft.graph.networkIPv4ConfigurationManagementCondition not found
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
    "id": "043f0ec8-0ec8-043f-c80e-3f04c80e3f04",
    "applicablePlatforms": [
      "String"
    ],
    "createdDateTime": "String (timestamp)",
    "description": "String",
    "displayName": "String",
    "eTag": "String",
    "modifiedDateTime": "String (timestamp)",
    "uniqueName": "String",
    "dnsSuffixList": [
      "String"
    ],
    "ipV4DHCPServer": "String",
    "ipV4DNSServerList": [
      "String"
    ],
    "ipV4Gateway": "String",
    "ipV4Prefix": "String"
  }
}
```


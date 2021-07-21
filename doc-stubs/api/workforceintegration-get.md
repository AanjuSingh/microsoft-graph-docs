---
title: "Get workforceIntegration"
description: "Read the properties and relationships of a workforceIntegration object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get workforceIntegration
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [workforceIntegration](../resources/workforceintegration.md) object.

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
GET /teamwork/workforceIntegrations/{workforceIntegrationId}
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

If successful, this method returns a `200 OK` response code and a [workforceIntegration](../resources/workforceintegration.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_workforceintegration"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/workforceIntegrations/{workforceIntegrationId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.workforceIntegration",
    "id": "f9015aa4-5aa4-f901-a45a-01f9a45a01f9",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "createdDateTime": "String (timestamp)",
    "lastModifiedBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "lastModifiedDateTime": "String (timestamp)",
    "apiVersion": "Integer",
    "displayName": "String",
    "eligibilityFilteringEnabledEntities": "String",
    "encryption": {
      "@odata.type": "microsoft.graph.workforceIntegrationEncryption"
    },
    "isActive": "Boolean",
    "supportedEntities": "String",
    "supports": "String",
    "url": "String"
  }
}
```


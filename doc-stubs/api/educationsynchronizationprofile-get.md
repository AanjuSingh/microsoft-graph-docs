---
title: "Get educationSynchronizationProfile"
description: "Read the properties and relationships of an educationSynchronizationProfile object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get educationSynchronizationProfile
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.

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
GET /education/synchronizationProfiles/{educationSynchronizationProfileId}
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

If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_educationsynchronizationprofile"
}
-->
``` http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{educationSynchronizationProfileId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
    "id": "ef555c1d-5c1d-ef55-1d5c-55ef1d5c55ef",
    "dataProvider": {
      "@odata.type": "microsoft.graph.educationSynchronizationDataProvider"
    },
    "displayName": "String",
    "expirationDate": "Date",
    "handleSpecialCharacterConstraint": "Boolean",
    "identitySynchronizationConfiguration": {
      "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration"
    },
    "licensesToAssign": [
      {
        "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment"
      }
    ],
    "state": "String"
  }
}
```


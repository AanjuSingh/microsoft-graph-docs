---
title: "Get person"
description: "Read the properties and relationships of a person object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get person
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of a [person](../resources/person.md) object.

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
GET /me/people/{personId}
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

If successful, this method returns a `200 OK` response code and a [person](../resources/person.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_person"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/people/{personId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.person"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.person",
    "id": "ac7d2783-2783-ac7d-8327-7dac83277dac",
    "birthday": "String",
    "companyName": "String",
    "department": "String",
    "displayName": "String",
    "emailAddresses": [
      {
        "@odata.type": "microsoft.graph.rankedEmailAddress"
      }
    ],
    "givenName": "String",
    "isFavorite": "Boolean",
    "mailboxType": "String",
    "officeLocation": "String",
    "personNotes": "String",
    "personType": "String",
    "phones": [
      {
        "@odata.type": "microsoft.graph.phone"
      }
    ],
    "postalAddresses": [
      {
        "@odata.type": "microsoft.graph.location"
      }
    ],
    "profession": "String",
    "sources": [
      {
        "@odata.type": "microsoft.graph.personDataSource"
      }
    ],
    "surname": "String",
    "title": "String",
    "userPrincipalName": "String",
    "websites": [
      {
        "@odata.type": "microsoft.graph.website"
      }
    ],
    "yomiCompany": "String"
  }
}
```


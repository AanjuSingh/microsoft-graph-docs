---
title: "List contacts"
description: "Get a list of the contact objects and their properties."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# List contacts
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Get a list of the [contact](../resources/contact.md) objects and their properties.

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
GET /me/contacts
GET /users/{usersId}/contacts
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

If successful, this method returns a `200 OK` response code and a collection of [contact](../resources/contact.md) objects in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "list_contact"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/contacts
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.contact)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.contact",
      "id": "d0f8f5eb-f5eb-d0f8-ebf5-f8d0ebf5f8d0",
      "categories": [
        "String"
      ],
      "changeKey": "String",
      "createdDateTime": "String (timestamp)",
      "lastModifiedDateTime": "String (timestamp)",
      "assistantName": "String",
      "birthday": "String (timestamp)",
      "children": [
        "String"
      ],
      "companyName": "String",
      "department": "String",
      "displayName": "String",
      "emailAddresses": [
        {
          "@odata.type": "microsoft.graph.typedEmailAddress"
        }
      ],
      "fileAs": "String",
      "flag": {
        "@odata.type": "microsoft.graph.followupFlag"
      },
      "gender": "String",
      "generation": "String",
      "givenName": "String",
      "imAddresses": [
        "String"
      ],
      "initials": "String",
      "isFavorite": "Boolean",
      "jobTitle": "String",
      "manager": "String",
      "middleName": "String",
      "nickName": "String",
      "officeLocation": "String",
      "parentFolderId": "String",
      "personalNotes": "String",
      "phones": [
        {
          "@odata.type": "microsoft.graph.phone"
        }
      ],
      "postalAddresses": [
        {
          "@odata.type": "microsoft.graph.physicalAddress"
        }
      ],
      "profession": "String",
      "spouseName": "String",
      "surname": "String",
      "title": "String",
      "websites": [
        {
          "@odata.type": "microsoft.graph.website"
        }
      ],
      "weddingAnniversary": "Date",
      "yomiCompanyName": "String",
      "yomiGivenName": "String",
      "yomiSurname": "String"
    }
  ]
}
```


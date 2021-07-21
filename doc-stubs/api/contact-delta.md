---
title: "contact: delta"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# contact: delta
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
GET /me/contacts/delta
GET /users/{usersId}/contacts/delta
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
Do not supply a request body for this method.

## Response

If successful, this function returns a `200 OK` response code and a [contact](../resources/contact.md) collection in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "contact_delta"
}
-->
``` http
GET https://graph.microsoft.com/beta/me/contacts/delta
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
      "id": "String (identifier)",
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


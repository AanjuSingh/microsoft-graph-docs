---
title: "List assignmentCategories"
description: "Retrieve a list of category objects."
author: "mmast-msft"
ms.localizationpriority: medium
ms.prod: "education"
doc_type: apiPageType
---

# List assignmentCategories

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Retrieve a list of [educationCategory](../resources/educationcategory.md) objects.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged)                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| Delegated (work or school account)     | EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite |
| Delegated (personal Microsoft account) | Not supported.                                                                                         |
| Application                            | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All |

## HTTP request

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## Optional query parameters

This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.

All [properties](/graph/api/resources/educationcategory#properties) are supported for `$filter`, `$orderby`.

## Request headers

| Header        | Value                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Do not supply a request body for this method.

## Response

If successful, this method returns a `200 OK` response code and a collection of [educationCategory](../resources/educationcategory.md) objects in the response body.

## Examples

### Example 1: Get assignment categories

### Request

The following is an example of the request.


# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["4797d052-ebf5-4018-a088-e11adc6b2cbb"],
  "name": "get_class_categories"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories
```

# [C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-class-categories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-class-categories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-class-categories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-class-categories-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# [PHP](#tab/php)
[!INCLUDE [sample-code](../includes/snippets/php/get-class-categories-php-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### Response

The following is an example of the response. 

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/education/classes('4797d052-ebf5-4018-a088-e11adc6b2cbb')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
          "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
      }
    ]
}
```

### Example 2: Using `$filter` to get assignment categories

#### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["2003c52e-807a-4186-9b49-60c573095461"],
  "name": "get_class_categories_filter"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2003c52e-807a-4186-9b49-60c573095461/assignmentCategories?$filter=id eq 'd4cb4f68-9136-48d3-9054-c1208ea274f0'
```

#### Response
The following is an example of the response. 

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('2003c52e-807a-4186-9b49-60c573095461')/assignmentCategories",
    "value": [
        {
            "displayName": "2022-11-09T20_16_24_105Z",
            "id": "d4cb4f68-9136-48d3-9054-c1208ea274f0"
        }
    ]
}
```

### Example 3: Using `$orderby` to get assignment categories

#### Request

The following is an example of the request.

# [HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["2003c52e-807a-4186-9b49-60c573095461"],
  "name": "get_class_categories_orderby"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/2003c52e-807a-4186-9b49-60c573095461/assignmentCategories?$orderby=displayName
```

#### Response
The following is an example of the response. 

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('2003c52e-807a-4186-9b49-60c573095461')/assignmentCategories",
    "@odata.nextLink": "https://graph.microsoft.com/beta/education/classes/2003c52e-807a-4186-9b49-60c573095461/assignmentCategories?$orderby=displayName&$skiptoken=MyZRVkZCUVVGQlFVRk5aelJCUVVGQlFVRkJRWGxCUVVGQlIyZE1VMjFyVFVrMk1HbFNablZPTXpkdVRpOVlkejA5",
    "value": [
        {
            "displayName": "2019-04-05T21_30_03_125Z",
            "id": "0c3c2de5-d317-42b9-a4a7-dede7a87f6df"
        },
        {
            "displayName": "2019-04-05T21_30_21'941Z",
            "id": "ec2a0bfe-f7c5-4a33-a5ea-58db087cb1c7"
        },
        {
            "displayName": "2019-04-17T18_46_15_996Z",
            "id": "5d4458a4-0784-491b-b4eb-643daf3408d0"
        },
        {
            "displayName": "2019-04-22T22_01_29_919Z",
            "id": "012c321e-70af-4b56-8949-1d228cbbdf35"
        },
        {
            "displayName": "2019-04-23T02_04_51_925Z",
            "id": "72fc6ce0-af91-4eaf-b675-b979aa7540c2"
        },
        {
            "displayName": "2019-04-24T18_24_54_540Z",
            "id": "3c8b14c1-a118-44fb-a308-8175f3dec179"
        },
        {
            "displayName": "2019-04-24T18_25_05_792Z",
            "id": "328b7715-86d4-4580-aae7-3dc80f570b49"
        },
        {
            "displayName": "2019-05-16T23_19_05_865Z",
            "id": "c71c2e76-4af4-4794-a6eb-fe86d30d9209"
        },
        {
            "displayName": "2019-05-16T23_19_06_340Z",
            "id": "29d62f01-1d70-447f-8c03-2ef19d3911f6"
        },
        {
            "displayName": "2019-05-16T23_19_06'504Z",
            "id": "63219333-859a-45f0-9003-bc1512b8c6a5"
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

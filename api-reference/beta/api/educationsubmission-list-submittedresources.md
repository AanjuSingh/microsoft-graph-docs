---
title: "List submittedResources"
description: "List the resources that have officially been submitted for grading. The student who owns the submission cannot change the submitted list without resubmitting the assignment. This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment."
author: "Sureshpadimi88"
ms.localizationpriority: medium
ms.prod: "education"
doc_type: apiPageType
---

# List submittedResources

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

List the [educationSubmissionResource](../resources/educationsubmissionresource.md) objects that have officially been submitted for grading. The student who owns the submission cannot change the submitted list without resubmitting the assignment. This is a wrapper around the real resource and can contain a pointer back to the actual assignment resource if this resource was copied from the assignment.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type      | Permissions (from least to most privileged)              |
|:--------------------|:---------------------------------------------------------|
|Delegated (work or school account) |  EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite  |
|Delegated (personal Microsoft account) |  Not supported.  |
|Application | EduAssignments.ReadBasic.All, EduAssignments.ReadWriteBasic.All, EduAssignments.Read.All, EduAssignments.ReadWrite.All | 

## HTTP request
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/submittedResources
```

## Optional query parameters

This method supports the `$top`, `$filter`, `$orderBy`, and `$select` OData query parameters to help customize the response. For general information, see [OData query parameters](/graph/query-parameters).

## Request headers
| Header       | Value |
|:---------------|:--------|
| Authorization  | Bearer {token}. Required.  |

## Request body
Do not supply a request body for this method.
## Response
If successful, this method returns a `200 OK` response code and a collection of [educationSubmissionResource](../resources/educationsubmissionresource.md) objects in the response body.
## Example

### Example 1: Get all submitted resources

#### Request
The following is an example of the request.
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/submittedResources
```
##### Response
The following is an example of the response. 

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
      "resource": {
          "@odata.type": "#microsoft.graph.educationLinkResource",
          "displayName": "Microsoft Homepage",
          "createdDateTime": "2017-10-21T07:52:45.5675913Z",
          "createdBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
          "lastModifiedBy": {
              "application": null,
              "device": null,
              "user": {
                  "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
                  "displayName": null
              }
          },
          "link": "https://www.microsoft.com"
      }
    }
  ]
}
```

### Example 2: Using `$filter` to get submitted resources

#### Request
The following is an example of the request.
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources_filter"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/2003c52e-807a-4186-9b49-60c573095461/assignments/03a893d4-f64b-47e4-9e0c-afac4b357007/submissions/be6280d6-cf92-d58e-6ca4-44babfcb2394/submittedResources?$filter=id eq '6d6e204d-d976-452e-a76b-14a43f77dc65'
```

##### Response
The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('2003c52e-807a-4186-9b49-60c573095461')/assignments('03a893d4-f64b-47e4-9e0c-afac4b357007')/submissions('be6280d6-cf92-d58e-6ca4-44babfcb2394')/submittedResources",
    "value": [
        {
            "assignmentResourceUrl": "https://assignments.onenote.com/api/v1.0/edu/classes/2003c52e-807a-4186-9b49-60c573095461/assignments/03a893d4-f64b-47e4-9e0c-afac4b357007/resources/45361b68-2777-42b1-aa4b-7054ce6de136",
            "id": "6d6e204d-d976-452e-a76b-14a43f77dc65",
            "resource": {
                "@odata.type": "#microsoft.graph.educationExternalResource",
                "displayName": "Forms Complete (Postman Test Dev)",
                "createdDateTime": "2022-04-13T02:00:32.0613061Z",
                "lastModifiedDateTime": "2022-04-13T02:00:32.0623064Z",
                "webUrl": "https://forms.office.com/Pages/AssignmentsDesignPage.aspx#TopView=Preview&FormId=kowztj5TbU-jJ5lCY3EjmS7FAyB6gIZBm0lgxXMJVGFUMVlZVFM2MDRCVk1NOFlRU0xJRExDWDVTQyQlQCN0PWcu",
                "createdBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "51cf5a99-d234-4e43-96de-cd65df14bfa1",
                        "displayName": null
                    }
                },
                "lastModifiedBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "51cf5a99-d234-4e43-96de-cd65df14bfa1",
                        "displayName": null
                    }
                }
            }
        }
    ]
}
```

### Example 2: Using `$orderby` to get submitted resources

#### Request
The following is an example of the request.
<!-- {
  "blockType": "ignored",
  "name": "get_submittedresources_orderby"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/2003c52e-807a-4186-9b49-60c573095461/assignments/03a893d4-f64b-47e4-9e0c-afac4b357007/submissions/be6280d6-cf92-d58e-6ca4-44babfcb2394/submittedResources?$orderby=id
```

##### Response
The following is an example of the response.

>**Note:** The response object shown here might be shortened for readability.

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationResource",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/classes('2003c52e-807a-4186-9b49-60c573095461')/assignments('03a893d4-f64b-47e4-9e0c-afac4b357007')/submissions('be6280d6-cf92-d58e-6ca4-44babfcb2394')/submittedResources",
    "value": [
        {
            "assignmentResourceUrl": "https://assignments.onenote.com/api/v1.0/edu/classes/2003c52e-807a-4186-9b49-60c573095461/assignments/03a893d4-f64b-47e4-9e0c-afac4b357007/resources/45361b68-2777-42b1-aa4b-7054ce6de136",
            "id": "6d6e204d-d976-452e-a76b-14a43f77dc65",
            "resource": {
                "@odata.type": "#microsoft.graph.educationExternalResource",
                "displayName": "Forms Complete (Postman Test Dev)",
                "createdDateTime": "2022-04-13T02:00:32.0613061Z",
                "lastModifiedDateTime": "2022-04-13T02:00:32.0623064Z",
                "webUrl": "https://forms.office.com/Pages/AssignmentsDesignPage.aspx#TopView=Preview&FormId=kowztj5TbU-jJ5lCY3EjmS7FAyB6gIZBm0lgxXMJVGFUMVlZVFM2MDRCVk1NOFlRU0xJRExDWDVTQyQlQCN0PWcu",
                "createdBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "51cf5a99-d234-4e43-96de-cd65df14bfa1",
                        "displayName": null
                    }
                },
                "lastModifiedBy": {
                    "application": null,
                    "device": null,
                    "user": {
                        "id": "51cf5a99-d234-4e43-96de-cd65df14bfa1",
                        "displayName": null
                    }
                }
            }
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submittedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

---
title: "Get employee"
description: "Read the properties and relationships of an employee object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Get employee
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Read the properties and relationships of an [employee](../resources/employee.md) object.

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
GET /financials/companies/{companyId}/employees/{employeeId}
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

If successful, this method returns a `200 OK` response code and an [employee](../resources/employee.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "get_employee"
}
-->
``` http
GET https://graph.microsoft.com/beta/financials/companies/{companyId}/employees/{employeeId}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.employee"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.employee",
    "id": "0d331309-1309-0d33-0913-330d0913330d",
    "address": {
      "@odata.type": "microsoft.graph.postalAddressType"
    },
    "birthDate": "Date",
    "displayName": "String",
    "email": "String",
    "employmentDate": "Date",
    "givenName": "String",
    "jobTitle": "String",
    "lastModifiedDateTime": "String (timestamp)",
    "middleName": "String",
    "mobilePhone": "String",
    "number": "String",
    "personalEmail": "String",
    "phoneNumber": "String",
    "statisticsGroupCode": "String",
    "status": "String",
    "surname": "String",
    "terminationDate": "Date"
  }
}
```


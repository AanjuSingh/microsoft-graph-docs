---
title: "Create office365ActiveUserDetail"
description: "Create a new office365ActiveUserDetail object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create office365ActiveUserDetail
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.

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
POST ** Collection URI for microsoft.graph.office365ActiveUserDetail not found
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object.

The following table shows the properties that are required when you create the [office365ActiveUserDetail](../resources/office365activeuserdetail.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|assignedProducts|String collection|**TODO: Add Description**|
|deletedDate|Date|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|exchangeLastActivityDate|Date|**TODO: Add Description**|
|exchangeLicenseAssignDate|Date|**TODO: Add Description**|
|hasExchangeLicense|Boolean|**TODO: Add Description**|
|hasOneDriveLicense|Boolean|**TODO: Add Description**|
|hasSharePointLicense|Boolean|**TODO: Add Description**|
|hasSkypeForBusinessLicense|Boolean|**TODO: Add Description**|
|hasTeamsLicense|Boolean|**TODO: Add Description**|
|hasYammerLicense|Boolean|**TODO: Add Description**|
|isDeleted|Boolean|**TODO: Add Description**|
|oneDriveLastActivityDate|Date|**TODO: Add Description**|
|oneDriveLicenseAssignDate|Date|**TODO: Add Description**|
|reportRefreshDate|Date|**TODO: Add Description**|
|sharePointLastActivityDate|Date|**TODO: Add Description**|
|sharePointLicenseAssignDate|Date|**TODO: Add Description**|
|skypeForBusinessLastActivityDate|Date|**TODO: Add Description**|
|skypeForBusinessLicenseAssignDate|Date|**TODO: Add Description**|
|teamsLastActivityDate|Date|**TODO: Add Description**|
|teamsLicenseAssignDate|Date|**TODO: Add Description**|
|userPrincipalName|String|**TODO: Add Description**|
|yammerLastActivityDate|Date|**TODO: Add Description**|
|yammerLicenseAssignDate|Date|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and an [office365ActiveUserDetail](../resources/office365activeuserdetail.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_office365activeuserdetail_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.graph.office365ActiveUserDetail not found
Content-Type: application/json
Content-length: 964

{
  "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
  "assignedProducts": [
    "String"
  ],
  "deletedDate": "Date",
  "displayName": "String",
  "exchangeLastActivityDate": "Date",
  "exchangeLicenseAssignDate": "Date",
  "hasExchangeLicense": "Boolean",
  "hasOneDriveLicense": "Boolean",
  "hasSharePointLicense": "Boolean",
  "hasSkypeForBusinessLicense": "Boolean",
  "hasTeamsLicense": "Boolean",
  "hasYammerLicense": "Boolean",
  "isDeleted": "Boolean",
  "oneDriveLastActivityDate": "Date",
  "oneDriveLicenseAssignDate": "Date",
  "reportRefreshDate": "Date",
  "sharePointLastActivityDate": "Date",
  "sharePointLicenseAssignDate": "Date",
  "skypeForBusinessLastActivityDate": "Date",
  "skypeForBusinessLicenseAssignDate": "Date",
  "teamsLastActivityDate": "Date",
  "teamsLicenseAssignDate": "Date",
  "userPrincipalName": "String",
  "yammerLastActivityDate": "Date",
  "yammerLicenseAssignDate": "Date"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserDetail"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.office365ActiveUserDetail",
  "id": "11ebd0cb-d0cb-11eb-cbd0-eb11cbd0eb11",
  "assignedProducts": [
    "String"
  ],
  "deletedDate": "Date",
  "displayName": "String",
  "exchangeLastActivityDate": "Date",
  "exchangeLicenseAssignDate": "Date",
  "hasExchangeLicense": "Boolean",
  "hasOneDriveLicense": "Boolean",
  "hasSharePointLicense": "Boolean",
  "hasSkypeForBusinessLicense": "Boolean",
  "hasTeamsLicense": "Boolean",
  "hasYammerLicense": "Boolean",
  "isDeleted": "Boolean",
  "oneDriveLastActivityDate": "Date",
  "oneDriveLicenseAssignDate": "Date",
  "reportRefreshDate": "Date",
  "sharePointLastActivityDate": "Date",
  "sharePointLicenseAssignDate": "Date",
  "skypeForBusinessLastActivityDate": "Date",
  "skypeForBusinessLicenseAssignDate": "Date",
  "teamsLastActivityDate": "Date",
  "teamsLicenseAssignDate": "Date",
  "userPrincipalName": "String",
  "yammerLastActivityDate": "Date",
  "yammerLicenseAssignDate": "Date"
}
```


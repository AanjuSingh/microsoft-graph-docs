---
title: "Create user"
description: "Create a new user object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create user
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Create a new [user](../resources/user.md) object.

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
POST /users
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [user](../resources/user.md) object.

You can specify the following properties when creating a **user**.

|Property|Type|Description|
|:---|:---|:---|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md). Optional.|
|aboutMe|String|**TODO: Add Description** Optional.|
|accountEnabled|Boolean|**TODO: Add Description** Optional.|
|ageGroup|String|**TODO: Add Description** Optional.|
|assignedLicenses|[assignedLicense](../resources/assignedlicense.md) collection|**TODO: Add Description** Required.|
|assignedPlans|[assignedPlan](../resources/assignedplan.md) collection|**TODO: Add Description** Required.|
|birthday|DateTimeOffset|**TODO: Add Description** Required.|
|businessPhones|String collection|**TODO: Add Description** Required.|
|city|String|**TODO: Add Description** Optional.|
|companyName|String|**TODO: Add Description** Optional.|
|consentProvidedForMinor|String|**TODO: Add Description** Optional.|
|country|String|**TODO: Add Description** Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|creationType|String|**TODO: Add Description** Optional.|
|customSecurityAttributes|[customSecurityAttributeValue](../resources/customsecurityattributevalue.md)|**TODO: Add Description** Optional.|
|department|String|**TODO: Add Description** Optional.|
|deviceEnrollmentLimit|Int32|The limit on the maximum number of devices that the user is permitted to enroll. Allowed values are 5 or 1000. Required.|
|deviceKeys|[deviceKey](../resources/devicekey.md) collection|**TODO: Add Description** Required.|
|displayName|String|**TODO: Add Description** Optional.|
|employeeHireDate|DateTimeOffset|**TODO: Add Description** Optional.|
|employeeId|String|**TODO: Add Description** Optional.|
|employeeOrgData|[employeeOrgData](../resources/employeeorgdata.md)|**TODO: Add Description** Optional.|
|employeeType|String|**TODO: Add Description** Optional.|
|externalUserState|String|**TODO: Add Description** Optional.|
|externalUserStateChangeDateTime|String|**TODO: Add Description** Optional.|
|faxNumber|String|**TODO: Add Description** Optional.|
|givenName|String|**TODO: Add Description** Optional.|
|hireDate|DateTimeOffset|**TODO: Add Description** Required.|
|identities|[objectIdentity](../resources/objectidentity.md) collection|**TODO: Add Description** Optional.|
|imAddresses|String collection|**TODO: Add Description** Optional.|
|infoCatalogs|String collection|**TODO: Add Description** Required.|
|interests|String collection|**TODO: Add Description** Optional.|
|isManagementRestricted|Boolean|**TODO: Add Description** Optional.|
|isResourceAccount|Boolean|**TODO: Add Description** Optional.|
|jobTitle|String|**TODO: Add Description** Optional.|
|lastPasswordChangeDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|legalAgeGroupClassification|String|**TODO: Add Description** Optional.|
|licenseAssignmentStates|[licenseAssignmentState](../resources/licenseassignmentstate.md) collection|**TODO: Add Description** Optional.|
|mail|String|**TODO: Add Description** Optional.|
|mailboxSettings|[mailboxSettings](../resources/mailboxsettings.md)|**TODO: Add Description** Optional.|
|mailNickname|String|**TODO: Add Description** Optional.|
|mobilePhone|String|**TODO: Add Description** Optional.|
|mySite|String|**TODO: Add Description** Optional.|
|officeLocation|String|**TODO: Add Description** Optional.|
|onPremisesDistinguishedName|String|**TODO: Add Description** Optional.|
|onPremisesDomainName|String|**TODO: Add Description** Optional.|
|onPremisesExtensionAttributes|[onPremisesExtensionAttributes](../resources/onpremisesextensionattributes.md)|**TODO: Add Description** Optional.|
|onPremisesImmutableId|String|**TODO: Add Description** Optional.|
|onPremisesLastSyncDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](../resources/onpremisesprovisioningerror.md) collection|**TODO: Add Description** Optional.|
|onPremisesSamAccountName|String|**TODO: Add Description** Optional.|
|onPremisesSecurityIdentifier|String|**TODO: Add Description** Optional.|
|onPremisesSyncEnabled|Boolean|**TODO: Add Description** Optional.|
|onPremisesUserPrincipalName|String|**TODO: Add Description** Optional.|
|otherMails|String collection|**TODO: Add Description** Required.|
|passwordPolicies|String|**TODO: Add Description** Optional.|
|passwordProfile|[passwordProfile](../resources/passwordprofile.md)|**TODO: Add Description** Optional.|
|pastProjects|String collection|**TODO: Add Description** Optional.|
|postalCode|String|**TODO: Add Description** Optional.|
|preferredDataLocation|String|**TODO: Add Description** Optional.|
|preferredLanguage|String|**TODO: Add Description** Optional.|
|preferredName|String|**TODO: Add Description** Optional.|
|provisionedPlans|[provisionedPlan](../resources/provisionedplan.md) collection|**TODO: Add Description** Required.|
|proxyAddresses|String collection|**TODO: Add Description** Required.|
|refreshTokensValidFromDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|responsibilities|String collection|**TODO: Add Description** Optional.|
|schools|String collection|**TODO: Add Description** Optional.|
|showInAddressList|Boolean|**TODO: Add Description** Optional.|
|signInActivity|[signInActivity](../resources/signinactivity.md)|**TODO: Add Description** Optional.|
|signInSessionsValidFromDateTime|DateTimeOffset|**TODO: Add Description** Optional.|
|skills|String collection|**TODO: Add Description** Optional.|
|state|String|**TODO: Add Description** Optional.|
|streetAddress|String|**TODO: Add Description** Optional.|
|surname|String|**TODO: Add Description** Optional.|
|temporaryAccessPass|[temporaryAccessPass](../resources/temporaryaccesspass.md)|**TODO: Add Description** Optional.|
|usageLocation|String|**TODO: Add Description** Optional.|
|userPrincipalName|String|**TODO: Add Description** Optional.|
|userType|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `201 Created` response code and a [user](../resources/user.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}
-->
``` http
POST https://graph.microsoft.com/beta/users
Content-Type: application/json
Content-length: 3636

{
  "@odata.type": "#microsoft.graph.user",
  "deletedDateTime": "String (timestamp)",
  "aboutMe": "String",
  "accountEnabled": "Boolean",
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "birthday": "String (timestamp)",
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "creationType": "String",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "department": "String",
  "deviceEnrollmentLimit": "Integer",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey"
    }
  ],
  "displayName": "String",
  "employeeHireDate": "String (timestamp)",
  "employeeId": "String",
  "employeeOrgData": {
    "@odata.type": "microsoft.graph.employeeOrgData"
  },
  "employeeType": "String",
  "externalUserState": "String",
  "externalUserStateChangeDateTime": "String",
  "faxNumber": "String",
  "givenName": "String",
  "hireDate": "String (timestamp)",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "infoCatalogs": [
    "String"
  ],
  "interests": [
    "String"
  ],
  "isManagementRestricted": "Boolean",
  "isResourceAccount": "Boolean",
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState"
    }
  ],
  "mail": "String",
  "mailboxSettings": {
    "@odata.type": "microsoft.graph.mailboxSettings"
  },
  "mailNickname": "String",
  "mobilePhone": "String",
  "mySite": "String",
  "officeLocation": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesDomainName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "pastProjects": [
    "String"
  ],
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "preferredName": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "responsibilities": [
    "String"
  ],
  "schools": [
    "String"
  ],
  "showInAddressList": "Boolean",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity"
  },
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "skills": [
    "String"
  ],
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "temporaryAccessPass": {
    "@odata.type": "microsoft.graph.temporaryAccessPass"
  },
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.user",
  "id": "4b7b9f2e-9f2e-4b7b-2e9f-7b4b2e9f7b4b",
  "deletedDateTime": "String (timestamp)",
  "aboutMe": "String",
  "accountEnabled": "Boolean",
  "ageGroup": "String",
  "assignedLicenses": [
    {
      "@odata.type": "microsoft.graph.assignedLicense"
    }
  ],
  "assignedPlans": [
    {
      "@odata.type": "microsoft.graph.assignedPlan"
    }
  ],
  "birthday": "String (timestamp)",
  "businessPhones": [
    "String"
  ],
  "city": "String",
  "companyName": "String",
  "consentProvidedForMinor": "String",
  "country": "String",
  "createdDateTime": "String (timestamp)",
  "creationType": "String",
  "customSecurityAttributes": {
    "@odata.type": "microsoft.graph.customSecurityAttributeValue"
  },
  "department": "String",
  "deviceEnrollmentLimit": "Integer",
  "deviceKeys": [
    {
      "@odata.type": "microsoft.graph.deviceKey"
    }
  ],
  "displayName": "String",
  "employeeHireDate": "String (timestamp)",
  "employeeId": "String",
  "employeeOrgData": {
    "@odata.type": "microsoft.graph.employeeOrgData"
  },
  "employeeType": "String",
  "externalUserState": "String",
  "externalUserStateChangeDateTime": "String",
  "faxNumber": "String",
  "givenName": "String",
  "hireDate": "String (timestamp)",
  "identities": [
    {
      "@odata.type": "microsoft.graph.objectIdentity"
    }
  ],
  "imAddresses": [
    "String"
  ],
  "infoCatalogs": [
    "String"
  ],
  "interests": [
    "String"
  ],
  "isManagementRestricted": "Boolean",
  "isResourceAccount": "Boolean",
  "jobTitle": "String",
  "lastPasswordChangeDateTime": "String (timestamp)",
  "legalAgeGroupClassification": "String",
  "licenseAssignmentStates": [
    {
      "@odata.type": "microsoft.graph.licenseAssignmentState"
    }
  ],
  "mail": "String",
  "mailboxSettings": {
    "@odata.type": "microsoft.graph.mailboxSettings"
  },
  "mailNickname": "String",
  "mobilePhone": "String",
  "mySite": "String",
  "officeLocation": "String",
  "onPremisesDistinguishedName": "String",
  "onPremisesDomainName": "String",
  "onPremisesExtensionAttributes": {
    "@odata.type": "microsoft.graph.onPremisesExtensionAttributes"
  },
  "onPremisesImmutableId": "String",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [
    {
      "@odata.type": "microsoft.graph.onPremisesProvisioningError"
    }
  ],
  "onPremisesSamAccountName": "String",
  "onPremisesSecurityIdentifier": "String",
  "onPremisesSyncEnabled": "Boolean",
  "onPremisesUserPrincipalName": "String",
  "otherMails": [
    "String"
  ],
  "passwordPolicies": "String",
  "passwordProfile": {
    "@odata.type": "microsoft.graph.passwordProfile"
  },
  "pastProjects": [
    "String"
  ],
  "postalCode": "String",
  "preferredDataLocation": "String",
  "preferredLanguage": "String",
  "preferredName": "String",
  "provisionedPlans": [
    {
      "@odata.type": "microsoft.graph.provisionedPlan"
    }
  ],
  "proxyAddresses": [
    "String"
  ],
  "refreshTokensValidFromDateTime": "String (timestamp)",
  "responsibilities": [
    "String"
  ],
  "schools": [
    "String"
  ],
  "showInAddressList": "Boolean",
  "signInActivity": {
    "@odata.type": "microsoft.graph.signInActivity"
  },
  "signInSessionsValidFromDateTime": "String (timestamp)",
  "skills": [
    "String"
  ],
  "state": "String",
  "streetAddress": "String",
  "surname": "String",
  "temporaryAccessPass": {
    "@odata.type": "microsoft.graph.temporaryAccessPass"
  },
  "usageLocation": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```


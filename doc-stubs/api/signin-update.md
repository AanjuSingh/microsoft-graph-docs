---
title: "Update signIn"
description: "Update the properties of a signIn object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update signIn
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [signIn](../resources/signin.md) object.

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
PATCH /auditLogs/signIns/{signInId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


|Property|Type|Description|
|:---|:---|:---|
|appDisplayName|String|**TODO: Add Description** Optional.|
|appId|String|**TODO: Add Description** Optional.|
|appliedConditionalAccessPolicies|[appliedConditionalAccessPolicy](../resources/appliedconditionalaccesspolicy.md) collection|**TODO: Add Description** Optional.|
|authenticationDetails|[authenticationDetail](../resources/authenticationdetail.md) collection|**TODO: Add Description** Optional.|
|authenticationMethodsUsed|String collection|**TODO: Add Description** Optional.|
|authenticationProcessingDetails|[keyValue](../resources/keyvalue.md) collection|**TODO: Add Description** Optional.|
|authenticationProtocol|protocolType|**TODO: Add Description**. The possible values are: `none`, `oAuth2`, `ropc`, `wsFederation`, `saml20`, `deviceCode`, `unknownFutureValue`. Optional.|
|authenticationRequirement|String|**TODO: Add Description** Optional.|
|authenticationRequirementPolicies|[authenticationRequirementPolicy](../resources/authenticationrequirementpolicy.md) collection|**TODO: Add Description** Optional.|
|autonomousSystemNumber|Int32|**TODO: Add Description** Optional.|
|clientAppUsed|String|**TODO: Add Description** Optional.|
|conditionalAccessStatus|conditionalAccessStatus|**TODO: Add Description**. The possible values are: `success`, `failure`, `notApplied`, `unknownFutureValue`. Optional.|
|correlationId|String|**TODO: Add Description** Optional.|
|createdDateTime|DateTimeOffset|**TODO: Add Description** Required.|
|crossTenantAccessType|signInAccessType|**TODO: Add Description**. The possible values are: `none`, `b2bCollaboration`, `b2bDirectConnect`, `microsoftSupport`, `serviceProvider`, `unknownFutureValue`. Optional.|
|deviceDetail|[deviceDetail](../resources/devicedetail.md)|**TODO: Add Description** Optional.|
|flaggedForReview|Boolean|**TODO: Add Description** Optional.|
|homeTenantId|String|**TODO: Add Description** Optional.|
|homeTenantName|String|**TODO: Add Description** Optional.|
|incomingTokenType|incomingTokenType|**TODO: Add Description**. The possible values are: `none`, `primaryRefreshToken`, `saml11`, `saml20`, `unknownFutureValue`. Optional.|
|ipAddress|String|**TODO: Add Description** Optional.|
|ipAddressFromResourceProvider|String|**TODO: Add Description** Optional.|
|isInteractive|Boolean|**TODO: Add Description** Optional.|
|isTenantRestricted|Boolean|**TODO: Add Description** Optional.|
|location|[signInLocation](../resources/signinlocation.md)|**TODO: Add Description** Optional.|
|mfaDetail|[mfaDetail](../resources/mfadetail.md)|**TODO: Add Description** Optional.|
|networkLocationDetails|[networkLocationDetail](../resources/networklocationdetail.md) collection|**TODO: Add Description** Optional.|
|originalRequestId|String|**TODO: Add Description** Optional.|
|privateLinkDetails|[privateLinkDetails](../resources/privatelinkdetails.md)|**TODO: Add Description** Optional.|
|processingTimeInMilliseconds|Int32|**TODO: Add Description** Optional.|
|resourceDisplayName|String|**TODO: Add Description** Optional.|
|resourceId|String|**TODO: Add Description** Optional.|
|resourceTenantId|String|**TODO: Add Description** Optional.|
|riskDetail|riskDetail|**TODO: Add Description**. The possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`. Optional.|
|riskEventTypes_v2|String collection|**TODO: Add Description** Optional.|
|riskLevelAggregated|riskLevel|**TODO: Add Description**. The possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Optional.|
|riskLevelDuringSignIn|riskLevel|**TODO: Add Description**. The possible values are: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Optional.|
|riskState|riskState|**TODO: Add Description**. The possible values are: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. Optional.|
|servicePrincipalCredentialKeyId|String|**TODO: Add Description** Optional.|
|servicePrincipalCredentialThumbprint|String|**TODO: Add Description** Optional.|
|servicePrincipalId|String|**TODO: Add Description** Required.|
|servicePrincipalName|String|**TODO: Add Description** Optional.|
|sessionLifetimePolicies|[sessionLifetimePolicy](../resources/sessionlifetimepolicy.md) collection|**TODO: Add Description** Optional.|
|signInEventTypes|String collection|**TODO: Add Description** Optional.|
|signInIdentifier|String|**TODO: Add Description** Optional.|
|signInIdentifierType|signInIdentifierType|**TODO: Add Description**. The possible values are: `userPrincipalName`, `phoneNumber`, `proxyAddress`, `qrCode`, `onPremisesUserPrincipalName`, `unknownFutureValue`. Optional.|
|status|[signInStatus](../resources/signinstatus.md)|**TODO: Add Description** Optional.|
|tokenIssuerName|String|**TODO: Add Description** Optional.|
|tokenIssuerType|tokenIssuerType|**TODO: Add Description**. The possible values are: `AzureAD`, `ADFederationServices`, `UnknownFutureValue`, `AzureADBackupAuth`. Note that you must use the `Prefer: include - unknown -enum-members` request header to get the following value(s) in this [evolvable enum](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations): `AzureADBackupAuth`. Optional.|
|uniqueTokenIdentifier|String|**TODO: Add Description** Optional.|
|userAgent|String|**TODO: Add Description** Optional.|
|userDisplayName|String|**TODO: Add Description** Optional.|
|userId|String|**TODO: Add Description** Required.|
|userPrincipalName|String|**TODO: Add Description** Optional.|
|userType|signInUserType|**TODO: Add Description**. The possible values are: `member`, `guest`, `unknownFutureValue`. Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [signIn](../resources/signin.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_signin"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/auditLogs/signIns/{signInId}
Content-Type: application/json
Content-length: 2661

{
  "@odata.type": "#microsoft.graph.signIn",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationProtocol": "String",
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "autonomousSystemNumber": "Integer",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "flaggedForReview": "Boolean",
  "homeTenantId": "String",
  "homeTenantName": "String",
  "incomingTokenType": "String",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "isInteractive": "Boolean",
  "isTenantRestricted": "Boolean",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "privateLinkDetails": {
    "@odata.type": "microsoft.graph.privateLinkDetails"
  },
  "processingTimeInMilliseconds": "Integer",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "riskDetail": "String",
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "servicePrincipalCredentialKeyId": "String",
  "servicePrincipalCredentialThumbprint": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "sessionLifetimePolicies": [
    {
      "@odata.type": "microsoft.graph.sessionLifetimePolicy"
    }
  ],
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "uniqueTokenIdentifier": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```


### Response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.signIn",
  "id": "040bde92-de92-040b-92de-0b0492de0b04",
  "appDisplayName": "String",
  "appId": "String",
  "appliedConditionalAccessPolicies": [
    {
      "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
    }
  ],
  "authenticationDetails": [
    {
      "@odata.type": "microsoft.graph.authenticationDetail"
    }
  ],
  "authenticationMethodsUsed": [
    "String"
  ],
  "authenticationProcessingDetails": [
    {
      "@odata.type": "microsoft.graph.keyValue"
    }
  ],
  "authenticationProtocol": "String",
  "authenticationRequirement": "String",
  "authenticationRequirementPolicies": [
    {
      "@odata.type": "microsoft.graph.authenticationRequirementPolicy"
    }
  ],
  "autonomousSystemNumber": "Integer",
  "clientAppUsed": "String",
  "conditionalAccessStatus": "String",
  "correlationId": "String",
  "createdDateTime": "String (timestamp)",
  "crossTenantAccessType": "String",
  "deviceDetail": {
    "@odata.type": "microsoft.graph.deviceDetail"
  },
  "flaggedForReview": "Boolean",
  "homeTenantId": "String",
  "homeTenantName": "String",
  "incomingTokenType": "String",
  "ipAddress": "String",
  "ipAddressFromResourceProvider": "String",
  "isInteractive": "Boolean",
  "isTenantRestricted": "Boolean",
  "location": {
    "@odata.type": "microsoft.graph.signInLocation"
  },
  "mfaDetail": {
    "@odata.type": "microsoft.graph.mfaDetail"
  },
  "networkLocationDetails": [
    {
      "@odata.type": "microsoft.graph.networkLocationDetail"
    }
  ],
  "originalRequestId": "String",
  "privateLinkDetails": {
    "@odata.type": "microsoft.graph.privateLinkDetails"
  },
  "processingTimeInMilliseconds": "Integer",
  "resourceDisplayName": "String",
  "resourceId": "String",
  "resourceTenantId": "String",
  "riskDetail": "String",
  "riskEventTypes_v2": [
    "String"
  ],
  "riskLevelAggregated": "String",
  "riskLevelDuringSignIn": "String",
  "riskState": "String",
  "servicePrincipalCredentialKeyId": "String",
  "servicePrincipalCredentialThumbprint": "String",
  "servicePrincipalId": "String",
  "servicePrincipalName": "String",
  "sessionLifetimePolicies": [
    {
      "@odata.type": "microsoft.graph.sessionLifetimePolicy"
    }
  ],
  "signInEventTypes": [
    "String"
  ],
  "signInIdentifier": "String",
  "signInIdentifierType": "String",
  "status": {
    "@odata.type": "microsoft.graph.signInStatus"
  },
  "tokenIssuerName": "String",
  "tokenIssuerType": "String",
  "uniqueTokenIdentifier": "String",
  "userAgent": "String",
  "userDisplayName": "String",
  "userId": "String",
  "userPrincipalName": "String",
  "userType": "String"
}
```


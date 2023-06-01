---
title: "cloudPcProvisioningPolicy: apply"
description: "Apply current provisioning policy configuration to all Cloud PC devices under a specified policy."
author: "Guoan-Tang"
ms.localizationpriority: medium
ms.prod: "cloud-pc"
doc_type: apiPageType
---

# cloudPcProvisioningPolicy: apply

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Apply current [provisioning policy](../resources/cloudpcprovisioningpolicy.md) configuration to all Cloud PC devices under a specified policy. Currently, you can only change the region.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|CloudPC.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|CloudPC.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies/{id}/apply
```

## Request headers

|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body

In the request body, supply a JSON representation of the parameters.

The following table shows the parameters that can be used with this method.

|Property|Type|Description|
|:---|:---|:---|
|`policySettings`|cloudPcPolicySettingType|The target property of this apply action. This property is a enum flag, possible values are: region, singleSignOn and their bitwise combination. Default value is `region` as action will only apply region change if this parameter is null.|

## Response

If successful, this method returns a `204 No Content` response code.

## Examples

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "apply_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/353b6a8e-67c5-4f68-8d89-4360487576c4/apply

{
  "policySettings": "region, singleSignOn"
}
```

### Response

The following is an example of the response.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
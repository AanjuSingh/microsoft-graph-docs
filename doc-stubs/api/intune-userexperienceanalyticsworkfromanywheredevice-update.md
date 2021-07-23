---
title: "Update userExperienceAnalyticsWorkFromAnywhereDevice"
description: "Update the properties of a userExperienceAnalyticsWorkFromAnywhereDevice object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update userExperienceAnalyticsWorkFromAnywhereDevice
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-userexperienceanalyticsworkfromanywheredevice.md) object.

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
PATCH /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-userexperienceanalyticsworkfromanywheredevice.md) object.

The following table shows the properties that are required when you update the [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-userexperienceanalyticsworkfromanywheredevice.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|deviceName|String|**TODO: Add Description**|
|serialNumber|String|**TODO: Add Description**|
|manufacturer|String|**TODO: Add Description**|
|model|String|**TODO: Add Description**|
|ownership|String|**TODO: Add Description**|
|managedBy|String|**TODO: Add Description**|
|autoPilotRegistered|Boolean|**TODO: Add Description**|
|autoPilotProfileAssigned|Boolean|**TODO: Add Description**|
|azureAdRegistered|Boolean|**TODO: Add Description**|
|azureAdDeviceId|String|**TODO: Add Description**|
|azureAdJoinType|String|**TODO: Add Description**|
|osDescription|String|**TODO: Add Description**|
|osVersion|String|**TODO: Add Description**|
|tenantAttached|Boolean|**TODO: Add Description**|
|compliancePolicySetToIntune|Boolean|**TODO: Add Description**|
|otherWorkloadsSetToIntune|Boolean|**TODO: Add Description**|
|upgradeEligibility|operatingSystemUpgradeEligibility|**TODO: Add Description**. Possible values are: `upgraded`, `unknown`, `notCapable`, `capable`.|
|ramCheckFailed|Boolean|**TODO: Add Description**|
|storageCheckFailed|Boolean|**TODO: Add Description**|
|processorCoreCountCheckFailed|Boolean|**TODO: Add Description**|
|processorSpeedCheckFailed|Boolean|**TODO: Add Description**|
|tpmCheckFailed|Boolean|**TODO: Add Description**|
|secureBootCheckFailed|Boolean|**TODO: Add Description**|
|processorFamilyCheckFailed|Boolean|**TODO: Add Description**|
|processor64BitCheckFailed|Boolean|**TODO: Add Description**|
|osCheckFailed|Boolean|**TODO: Add Description**|



## Response

If successful, this method returns a `200 OK` response code and an updated [userExperienceAnalyticsWorkFromAnywhereDevice](../resources/intune-userexperienceanalyticsworkfromanywheredevice.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_userexperienceanalyticsworkfromanywheredevice"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics/{userExperienceAnalyticsWorkFromAnywhereMetricId}/metricDevices/{userExperienceAnalyticsWorkFromAnywhereDeviceId}
Content-Type: application/json
Content-length: 982

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": "Boolean",
  "autoPilotProfileAssigned": "Boolean",
  "azureAdRegistered": "Boolean",
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String",
  "osDescription": "String",
  "osVersion": "String",
  "tenantAttached": "Boolean",
  "compliancePolicySetToIntune": "Boolean",
  "otherWorkloadsSetToIntune": "Boolean",
  "upgradeEligibility": "String",
  "ramCheckFailed": "Boolean",
  "storageCheckFailed": "Boolean",
  "processorCoreCountCheckFailed": "Boolean",
  "processorSpeedCheckFailed": "Boolean",
  "tpmCheckFailed": "Boolean",
  "secureBootCheckFailed": "Boolean",
  "processorFamilyCheckFailed": "Boolean",
  "processor64BitCheckFailed": "Boolean",
  "osCheckFailed": "Boolean"
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
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereDevice",
  "id": "4c29fe4a-fe4a-4c29-4afe-294c4afe294c",
  "deviceName": "String",
  "serialNumber": "String",
  "manufacturer": "String",
  "model": "String",
  "ownership": "String",
  "managedBy": "String",
  "autoPilotRegistered": "Boolean",
  "autoPilotProfileAssigned": "Boolean",
  "azureAdRegistered": "Boolean",
  "azureAdDeviceId": "String",
  "azureAdJoinType": "String",
  "osDescription": "String",
  "osVersion": "String",
  "tenantAttached": "Boolean",
  "compliancePolicySetToIntune": "Boolean",
  "otherWorkloadsSetToIntune": "Boolean",
  "upgradeEligibility": "String",
  "ramCheckFailed": "Boolean",
  "storageCheckFailed": "Boolean",
  "processorCoreCountCheckFailed": "Boolean",
  "processorSpeedCheckFailed": "Boolean",
  "tpmCheckFailed": "Boolean",
  "secureBootCheckFailed": "Boolean",
  "processorFamilyCheckFailed": "Boolean",
  "processor64BitCheckFailed": "Boolean",
  "osCheckFailed": "Boolean"
}
```


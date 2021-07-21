---
title: "Update deviceHealthScriptRunSummary"
description: "Update the properties of a deviceHealthScriptRunSummary object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Update deviceHealthScriptRunSummary
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.

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
PATCH /deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object.

The following table shows the properties that are required when you update the [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|detectionScriptErrorDeviceCount|Int32|Number of devices on which the detection script execution encountered an error and did not complete|
|detectionScriptNotApplicableDeviceCount|Int32|Number of devices for which the detection script was not applicable|
|detectionScriptPendingDeviceCount|Int32|Number of devices which have not yet run the latest version of the device health script|
|issueDetectedDeviceCount|Int32|Number of devices for which the detection script found an issue|
|issueRemediatedCumulativeDeviceCount|Int32|Number of devices that were remediated over the last 30 days|
|issueRemediatedDeviceCount|Int32|Number of devices for which the remediation script was able to resolve the detected issue|
|issueReoccurredDeviceCount|Int32|Number of devices for which the remediation script executed successfully but failed to resolve the detected issue|
|lastScriptRunDateTime|DateTimeOffset|Last run time for the script across all devices|
|noIssueDetectedDeviceCount|Int32|Number of devices for which the detection script did not find an issue and the device is healthy|
|remediationScriptErrorDeviceCount|Int32|Number of devices for which the remediation script execution encountered an error and did not complete|
|remediationSkippedDeviceCount|Int32|Number of devices for which remediation was skipped|



## Response

If successful, this method returns a `200 OK` response code and an updated [deviceHealthScriptRunSummary](../resources/devicehealthscriptrunsummary.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "update_devicehealthscriptrunsummary"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceHealthScripts/{deviceHealthScriptId}/runSummary
Content-Type: application/json
Content-length: 603

{
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "detectionScriptErrorDeviceCount": "Integer",
  "detectionScriptNotApplicableDeviceCount": "Integer",
  "detectionScriptPendingDeviceCount": "Integer",
  "issueDetectedDeviceCount": "Integer",
  "issueRemediatedCumulativeDeviceCount": "Integer",
  "issueRemediatedDeviceCount": "Integer",
  "issueReoccurredDeviceCount": "Integer",
  "lastScriptRunDateTime": "String (timestamp)",
  "noIssueDetectedDeviceCount": "Integer",
  "remediationScriptErrorDeviceCount": "Integer",
  "remediationSkippedDeviceCount": "Integer"
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
  "@odata.type": "#microsoft.graph.deviceHealthScriptRunSummary",
  "id": "1ebee6cb-e6cb-1ebe-cbe6-be1ecbe6be1e",
  "detectionScriptErrorDeviceCount": "Integer",
  "detectionScriptNotApplicableDeviceCount": "Integer",
  "detectionScriptPendingDeviceCount": "Integer",
  "issueDetectedDeviceCount": "Integer",
  "issueRemediatedCumulativeDeviceCount": "Integer",
  "issueRemediatedDeviceCount": "Integer",
  "issueReoccurredDeviceCount": "Integer",
  "lastScriptRunDateTime": "String (timestamp)",
  "noIssueDetectedDeviceCount": "Integer",
  "remediationScriptErrorDeviceCount": "Integer",
  "remediationSkippedDeviceCount": "Integer"
}
```


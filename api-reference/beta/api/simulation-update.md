---
title: "Update simulation"
description: "Update an attack simulation campaign for a tenant."
author: "stuartcl"
ms.localizationpriority: medium
ms.prod: "security"
doc_type: apiPageType
---

# Update simulation

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update an attack simulation campaign for a tenant.

## Permissions

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Permission type                        | Permissions (from least to most privileged) |
|:---------------------------------------|:--------------------------------------------|
| Delegated (work or school account)     | AttackSimulation.ReadWrite.All              |
| Delegated (personal Microsoft account) | Not supported.                              |
| Application                            | AttackSimulation.ReadWrite.All              |

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
```http
PATCH /security/attackSimulation/simulations/{simulationId}
```

## Request headers

|Header         |Value                    |
|---------------|-------------------------|
|Authorization  |Bearer {token}. Required.|
|Content-Type   |application/json         |

## Request body

[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]

|Property|Type|Description|
|:---|:---|:---|
|id|String|Simulation Id|
|attackTechnique|[simulationAttackTechnique](../resources/simulation.md#simulationattacktechnique-values)|The social engineering technique used in the attack simulation and training campaign. Supports `$filter` and `$orderby`. Possible values are: `unknown`, `credentialHarvesting`, `attachmentMalware`, `driveByUrl`, `linkInAttachment`, `linkToMalwareFile`, `unknownFutureValue`. For more information on the types of social engineering attack techniques, see [simulations](/microsoft-365/security/office-365-security/attack-simulation-training-get-started?view=o365-worldwide&preserve-view=true#simulations).|
|attackType|[simulationAttackType](../resources/simulation.md#simulationattacktype-values)|Attack type of the attack simulation and training campaign. Supports `$filter` and `$orderby`. Possible values are: `unknown`, `social`, `cloud`, `endpoint`, `unknownFutureValue`.|
|displayName|String|Display name of the attack simulation and training campaign. Supports `$filter` and `$orderby`.|
|durationInDays|Int32|Simulation duration in days.|
|excludedAccountTarget|[accountTargetContent](../resources/accounttargetcontent.md)|Users excluded from the simulation.|
|includedAccountTarget|[accountTargetContent](../resources/accounttargetcontent.md)|Users targeted in the simulation.|
|payload|[payload](../resources/payload.md)|Payload associated with the simulation.|
|status|[simulationStatus](../resources/simulation.md#simulationstatus-values)|Status of the attack simulation and training campaign. Supports `$filter` and `$orderby`. Possible values are: `unknown`, `draft`, `running`, `scheduled`, `succeeded`, `failed`, `cancelled`, `excluded`, `unknownFutureValue`.|

## Response

If successful, this method returns a `202 Accepted` response code and a tracking header named `location` in the response.

## Examples

### Request

The following is an example of a request.

<!-- {
  "blockType": "request",
  "name": "update_simulation",
  "sampleKeys": ["2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc"]
}
-->
```http
PATCH https://graph.microsoft.com/beta/security/attackSimulation/simulations/2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc
Content-type: application/json

{
  "@odata.etag": "\"0100aa9b-0000-0100-0000-6396fa270000\"",
  "id": "2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc",
  "displayName": "Graph Simulation",
  "payload@odata.bind":"https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a",
  "durationInDays": 7,
  "attackTechnique": "credentialHarvesting",
  "attackType": "social",
  "status": "scheduled",
  "includedAccountTarget": {
    "@odata.type": "#microsoft.graph.addressBookAccountTargetContent",
    "type" : "addressBook",
    "accountTargetEmails" : [
        "faiza@contoso.com"
    ]
  },
  "excludedAccountTarget": {
    "@odata.type": "#microsoft.graph.addressBookAccountTargetContent",
    "type" : "addressBook",
    "accountTargetEmails" : [
        "sam@contoso.com"
    ]
  }
}
```

### Response

The following is an example of the response.

> **Note**: The response object shown here might be shortened for readability.

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 202 Accepted
```


### Example

####Example 1: Update simulation from draft to scheduled
Simulation reques is validated during scheduling a simulation. All the required parameters need to be propogated in such request.

```http
PATCH https://graph.microsoft.com/beta/security/attackSimulation/simulations/2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc
Content-type: application/json

{
  "@odata.etag": "\"0100aa9b-0000-0100-0000-6396fa270000\"",
  "id": "2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc",
  "displayName": "Graph Simulation",
  "payload@odata.bind":"https://graph.microsoft.com/beta/security/attacksimulation/payloads/12345678-9abc-def0-123456789a",
  "durationInDays": 7,
  "attackTechnique": "credentialHarvesting",
  "attackType": "social",
  "status": "scheduled",
  "includedAccountTarget": {
    "@odata.type": "#microsoft.graph.addressBookAccountTargetContent",
    "type" : "addressBook",
    "accountTargetEmails" : [
        "faiza@contoso.com"
    ]
  },
  "excludedAccountTarget": {
    "@odata.type": "#microsoft.graph.addressBookAccountTargetContent",
    "type" : "addressBook",
    "accountTargetEmails" : [
        "sam@contoso.com"
    ]
  }
}
```

### Response

-->
```http
HTTP/1.1 202 Accepted
```

####Example 2: Cancelling a simulation
A simulation can be cancelled from `scheduled` and `running` state.

```http
PATCH https://graph.microsoft.com/beta/security/attackSimulation/simulations/2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc
Content-type: application/json

{
  "@odata.etag": "\"0100aa9b-0000-0100-0000-6396fa270000\"",
  "id": "2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc",
  "status": "cancelled"
}
```

### Response

-->
```http
HTTP/1.1 202 Accepted
```


####Example 3: Excluding a simulation
A simulation can be excluded from any reporting for simulation is `cancelled` state only.
```http
PATCH https://graph.microsoft.com/beta/security/attackSimulation/simulations/2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc
Content-type: application/json

{
  "@odata.etag": "\"0100aa9b-0000-0100-0000-6396fa270000\"",
  "id": "2f5548d1-0dd8-4cc8-9de0-e0d6ec7ea3dc",
  "status": "excluded"
}
```

### Response

-->
```http
HTTP/1.1 202 Accepted
```
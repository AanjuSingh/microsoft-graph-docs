---
title: "accessPackageAssignment resource type"
description: "An access package assignment is an assignment of an access package to a particular subject, for a period of time."
author: "markwahl-msft"
ms.localizationpriority: medium
ms.prod: "governance"
doc_type: resourcePageType
---
# accessPackageAssignment resource type

Namespace: microsoft.graph

In [Azure AD Entitlement Management](entitlementmanagement-root.md), an access package assignment is an assignment of an access package to a particular subject, for a period of time.  For example, an access package assignment can state that user Alice has been assigned access via the access package Sales for the period January 2019 through July 2019.


## Methods
|Method|Return type|Description|
|:---|:---|:---|
|[List accessPackageAssignments](../api/entitlementmanagement-list-assignments.md)|[accessPackageAssignment](accesspackageassignment.md) collection|Retrieve a list of **accessPackageAssignment** objects. |
|[filterByCurrentUser](../api/accesspackageassignment-filterbycurrentuser.md)|[accessPackageAssignment](../resources/accesspackageassignment.md) collection|Retrieve the list of **accessPackageAssignment** objects filtered on the signed-in user.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|expiredDateTime|DateTimeOffset|The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.|
|id|String|Read-only.|
|schedule|[entitlementManagementSchedule](../resources/entitlementmanagementschedule.md)|When the access assignment is to be in place. Read-only.|
|state|accessPackageAssignmentState|The state of the access package assignment. The possible values are: `delivering`, `partiallyDelivered`, `delivered`, `expired`, `deliveryFailed`, `unknownFutureValue`. Read-only.|
|status|String|More information about the assignment lifecycle.  Possible values include `Delivering`, `Delivered`, `NearExpiry1DayNotificationTriggered`, or `ExpiredNotificationTriggered`.  Read-only.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|accessPackage|[accessPackage](accesspackage.md)|Read-only. Nullable.|
|target|[accessPackageSubject](accesspackagesubject.md)|The subject of the access package assignment. Read-only. Nullable.|

## JSON representation
The following is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageAssignment",
  "id": "String (identifier)",
  "state": "String",
  "status": "String",
  "expiredDateTime": "String (timestamp)",
  "schedule": {
    "@odata.type": "microsoft.graph.entitlementManagementSchedule"
  }
}
```



---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcSnapshotIdRequestBody
{
	CloudPcSnapshotId = "A00009UV000_93aff428-61f2-467f-a879-1102af6fd4a8",
};
await graphClient.DeviceManagement.ManagedDevices["managedDevice-id"].RestoreCloudPc.PostAsync(requestBody);


```
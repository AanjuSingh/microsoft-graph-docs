---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CloudPcProvisioningPolicy
{
	@odata.type = "#microsoft.graph.cloudPcProvisioningPolicy",
	DisplayName = "HR provisioning policy",
	Description = "Provisioning policy for India HR employees",
	OnPremisesConnectionId = "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
	ImageId = "Image ID value",
	ImageDisplayName = "Image Display Name value",
	ImageType = "custom",
	WindowsSettings = new CloudPcWindowsSettings
	{
		Language = "en-US",
	},
};
await graphClient.DeviceManagement.VirtualEndpoint.ProvisioningPolicies["cloudPcProvisioningPolicy-id"].PatchAsync(requestBody);


```
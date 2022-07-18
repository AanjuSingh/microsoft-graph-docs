---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NewAssignmentOrderRequestBody
{
	NewAssignmentOrder = new AssignmentOrder
	{
		Order = new List<String>
		{
			"City",
			"extension_GUID_ShoeSize",
		}
	},
};
await graphClient.Identity.B2xUserFlows["b2xIdentityUserFlow-id"].UserAttributeAssignments.SetOrder.PostAsync(requestBody);


```
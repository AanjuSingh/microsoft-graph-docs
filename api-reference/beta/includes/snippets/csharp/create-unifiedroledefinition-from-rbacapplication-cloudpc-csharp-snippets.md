---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleDefinition
{
	Description = "An example custom role",
	DisplayName = "ExampleCustomRole",
	RolePermissions = new List<UnifiedRolePermission>
	{
		new UnifiedRolePermission
		{
			AdditionalData = new()
			{
				{"allowedResourceActions", new List<String>
				{
					"Microsoft.CloudPC/CloudPCs/Read",
				}
			}
		},
	}
	AdditionalData = new()
	{
		{"condition", "null"},
	}
};
var result = await graphClient.RoleManagement.CloudPC.RoleDefinitions.PostAsync(requestBody);


```
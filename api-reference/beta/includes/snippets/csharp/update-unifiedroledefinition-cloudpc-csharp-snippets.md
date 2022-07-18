---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleDefinition
{
	Description = "Update basic properties and permission of application registrations",
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
					"Microsoft.CloudPC/CloudPCs/Reprovision",
				}
			}
		},
	}
};
await graphClient.RoleManagement.CloudPC.RoleDefinitions["unifiedRoleDefinition-id"].PatchAsync(requestBody);


```
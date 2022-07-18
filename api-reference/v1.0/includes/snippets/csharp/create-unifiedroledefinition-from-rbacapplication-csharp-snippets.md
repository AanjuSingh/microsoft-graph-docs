---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new UnifiedRoleDefinition
{
	Description = "Update basic properties of application registrations",
	DisplayName = "Application Registration Support Administrator",
	RolePermissions = new List<UnifiedRolePermission>
	{
		new UnifiedRolePermission
		{
			AdditionalData = new()
			{
				{"allowedResourceActions", new List<String>
				{
					"microsoft.directory/applications/basic/read",
				}
			}
		},
	}
	IsEnabled = true,
};
var result = await graphClient.RoleManagement.Directory.RoleDefinitions.PostAsync(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageResourceRoleScope
{
	AccessPackageResourceRole = new 
	{
		OriginId = "Member_b31fe1f1-3651-488f-bd9a-1711887fd4ca",
		DisplayName = "Member",
		OriginSystem = "AadGroup",
		AccessPackageResource = new 
		{
			Id = "1d08498d-72a1-403f-8511-6b1f875746a0",
			ResourceType = "O365 Group",
			OriginId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca",
			OriginSystem = "AadGroup",
		},
	},
	AccessPackageResourceScope = new 
	{
		OriginId = "b31fe1f1-3651-488f-bd9a-1711887fd4ca",
		OriginSystem = "AadGroup",
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackages["accessPackage-id"].AccessPackageResourceRoleScopes.PostAsync(requestBody);


```
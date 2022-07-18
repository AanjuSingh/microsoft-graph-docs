---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentRequest
{
	RequestType = "AdminAdd",
	Assignment = new 
	{
		AdditionalData = new()
		{
			{"targetId", "46184453-e63b-4f20-86c2-c557ed5d5df9"},
			{"assignmentPolicyId", "2264bf65-76ba-417b-a27d-54d291f0cbc8"},
			{"accessPackageId", "a914b616-e04e-476b-aa37-91038f0b165b"},
		}
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AssignmentRequests.PostAsync(requestBody);


```
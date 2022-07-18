---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessPackageAssignmentRequest
{
	RequestType = "UserAdd",
	AccessPackageAssignment = new 
	{
		TargetId = "46184453-e63b-4f20-86c2-c557ed5d5df9",
		AssignmentPolicyId = "2264bf65-76ba-417b-a27d-54d291f0cbc8",
		AccessPackageId = "a914b616-e04e-476b-aa37-91038f0b165b",
	},
	Answers = new List<AccessPackageAnswer>
	{
		new AccessPackageAnswer
		{
			@odata.type = "#microsoft.graph.accessPackageAnswerString",
			AnsweredQuestion = new AccessPackageQuestion
			{
				@odata.type = "#microsoft.graph.accessPackageMultipleChoiceQuestion",
				Id = "A714EC6F-4EE0-4614-BD81-37E0C5ECBBFF",
			},
			AdditionalData = new()
			{
				{"value", "Arizona"},
			}
		},
		new AccessPackageAnswer
		{
			@odata.type = "#microsoft.graph.accessPackageAnswerString",
			AnsweredQuestion = new AccessPackageQuestion
			{
				@odata.type = "#microsoft.graph.accessPackageTextInputQuestion",
				Id = "AA615EE9-D9D8-4C03-BE91-BEE37106DEDA",
			},
			AdditionalData = new()
			{
				{"value", "Need access to marketing campaign material"},
			}
		},
	}
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageAssignmentRequests.PostAsync(requestBody);


```
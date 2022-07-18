---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationAssignmentResource
{
	DistributeForStudentWork = false,
	Resource = new EducationResource
	{
		@odata.type = "microsoft.graph.educationPowerPointResource",
		DisplayName = "state diagram.pptx",
		AdditionalData = new()
		{
			{"fileUrl", "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RN327OXRN6EVFE2Q5FRJZTN5EOJ"},
		}
	},
};
var result = await graphClient.Education.Classes["educationClass-id"].Assignments["educationAssignment-id"].Resources.PostAsync(requestBody);


```
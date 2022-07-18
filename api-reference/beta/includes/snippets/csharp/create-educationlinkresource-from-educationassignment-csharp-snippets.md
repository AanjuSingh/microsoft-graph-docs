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
		DisplayName = "Where the Wonders of Learning Never Cease | Wonderopolis",
		@odata.type = "#microsoft.graph.educationLinkResource",
		AdditionalData = new()
		{
			{"link", "https://wonderopolis.org/"},
			{"thumbnailPreviewUrl", null},
		}
	},
};
var result = await graphClient.Education.Classes["educationClass-id"].Assignments["educationAssignment-id"].Resources.PostAsync(requestBody);


```
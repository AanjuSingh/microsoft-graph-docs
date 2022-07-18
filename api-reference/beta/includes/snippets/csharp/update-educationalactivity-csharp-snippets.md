---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EducationalActivity
{
	Institution = new InstitutionData
	{
		Location = new PhysicalAddress
		{
			Type = "business",
			PostOfficeBox = null,
			Street = "12000 E Prospect Rd",
			City = "Fort Collins",
			State = "Colorado",
			CountryOrRegion = "USA",
			PostalCode = "80525",
		},
	},
};
await graphClient.Me.Profile.EducationalActivities["educationalActivity-id"].PatchAsync(requestBody);


```
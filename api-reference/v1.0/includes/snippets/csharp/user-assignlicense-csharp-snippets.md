---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AssignLicenseRequestBody
{
	AddLicenses = new List<AssignedLicense>
	{
		new AssignedLicense
		{
			AdditionalData = new()
			{
				{"disabledPlans", new List<String>
				{
					"11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
				}
				{"skuId", "45715bb8-13f9-4bf6-927f-ef96c102d394"},
			}
		},
	}
	RemoveLicenses = new List<String>
	{
		"bea13e0c-3828-4daa-a392-28af7ff61a0f",
	}
};
var result = await graphClient.Me.AssignLicense.PostAsync(requestBody);


```
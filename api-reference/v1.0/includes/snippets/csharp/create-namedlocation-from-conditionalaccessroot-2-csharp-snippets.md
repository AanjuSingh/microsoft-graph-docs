---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new NamedLocation
{
	@odata.type = "#microsoft.graph.countryNamedLocation",
	DisplayName = "Named location with unknown countries and regions",
	AdditionalData = new()
	{
		{"countriesAndRegions", new List<String>
		{
			"US",
			"GB",
		}
		{"includeUnknownCountriesAndRegions", true},
	}
};
var result = await graphClient.Identity.ConditionalAccess.NamedLocations.PostAsync(requestBody);


```
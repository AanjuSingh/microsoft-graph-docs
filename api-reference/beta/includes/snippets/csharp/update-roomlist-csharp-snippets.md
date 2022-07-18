---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Place
{
	@odata.type = "microsoft.graph.roomList",
	DisplayName = "Building 1",
	Phone = "555-555-0100",
	Address = new PhysicalAddress
	{
		Street = "4567 Main Street",
		City = "Buffalo",
		State = "NY",
		PostalCode = "98052",
		CountryOrRegion = "USA",
	},
	GeoCoordinates = new OutlookGeoCoordinates
	{
		Altitude = null,
		Latitude = 47d,
		Longitude = -122d,
		Accuracy = null,
		AltitudeAccuracy = null,
	},
};
await graphClient.Places["place-id"].PatchAsync(requestBody);


```
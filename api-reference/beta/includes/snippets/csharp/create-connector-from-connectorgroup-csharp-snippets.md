---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReferenceCreate
{
	@odata.id = "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}",
};
await graphClient.OnPremisesPublishingProfiles["onPremisesPublishingProfile-id"].ConnectorGroups["connectorGroup-id"].Members.$ref.PostAsync(requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new InferenceClassificationOverride
{
	ClassifyAs = "focused",
};
await graphClient.Me.InferenceClassification.Overrides["inferenceClassificationOverride-id"].PatchAsync(requestBody);


```
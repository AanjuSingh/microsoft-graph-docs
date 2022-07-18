---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new BatchRecordDecisionsRequestBody
{
	Decision = "Approve",
	Justification = "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
	ResourceId = "a5c51e59-3fcd-4a37-87a1-835c0c21488a",
};
await graphClient.IdentityGovernance.AccessReviews.Definitions["accessReviewScheduleDefinition-id"].Instances["accessReviewInstance-id"].BatchRecordDecisions.PostAsync(requestBody);


```
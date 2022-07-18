---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ChatMessage
{
	PolicyViolation = new ChatMessagePolicyViolation
	{
		PolicyTip = new ChatMessagePolicyViolationPolicyTip
		{
			GeneralText = "This item has been blocked by the administrator.",
			ComplianceUrl = "https://contoso.com/dlp-policy-page",
			MatchedConditionDescriptions = new List<String>
			{
				"Credit Card Number",
			}
		},
		VerdictDetails = "AllowOverrideWithoutJustification,AllowFalsePositiveOverride",
		DlpAction = "BlockAccess",
	},
};
await graphClient.Teams["team-id"].Channels["channel-id"].Messages["chatMessage-id"].PatchAsync(requestBody);


```
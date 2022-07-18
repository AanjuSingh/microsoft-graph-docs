---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AccessReviewScheduleDefinition
{
	DisplayName = "Group Multi-stage Access Review",
	DescriptionForAdmins = "New scheduled access review",
	DescriptionForReviewers = "If you have any questions, contact jerry@contoso.com",
	Scope = new AccessReviewScope
	{
		@odata.type = "#microsoft.graph.accessReviewQueryScope",
		AdditionalData = new()
		{
			{"query", "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers"},
			{"queryType", "MicrosoftGraph"},
		}
	},
	StageSettings = new List<AccessReviewStageSettings>
	{
		new AccessReviewStageSettings
		{
			StageId = "1",
			DurationInDays = 2,
			RecommendationsEnabled = false,
			DecisionsThatWillMoveToNextStage = new List<String>
			{
				"NotReviewed",
				"Approve",
			}
			Reviewers = new List<Object>
			{
				new 
				{
					AdditionalData = new()
					{
						{"query", "/users/398164b1-5196-49dd-ada2-364b49f99b27"},
						{"queryType", "MicrosoftGraph"},
					}
				},
			}
		},
		new AccessReviewStageSettings
		{
			StageId = "2",
			DependsOn = new List<String>
			{
				"1",
			}
			DurationInDays = 2,
			RecommendationsEnabled = true,
			Reviewers = new List<Object>
			{
				new 
				{
					AdditionalData = new()
					{
						{"query", "./manager"},
						{"queryType", "MicrosoftGraph"},
						{"queryRoot", "decisions"},
					}
				},
			}
			FallbackReviewers = new List<Object>
			{
				new 
				{
					AdditionalData = new()
					{
						{"query", "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers"},
						{"queryType", "MicrosoftGraph"},
					}
				},
			}
		},
	}
	Settings = new AccessReviewScheduleSettings
	{
		MailNotificationsEnabled = true,
		ReminderNotificationsEnabled = true,
		JustificationRequiredOnApproval = true,
		DefaultDecisionEnabled = false,
		DefaultDecision = "None",
		InstanceDurationInDays = 4,
		Recurrence = new PatternedRecurrence
		{
			Pattern = new RecurrencePattern
			{
				Type = "weekly",
				Interval = 1,
			},
			Range = new RecurrenceRange
			{
				Type = "noEnd",
				StartDate = "2020-09-08T12:02:30.667Z",
			},
		},
		DecisionHistoriesForReviewersEnabled = true,
	},
};
var result = await graphClient.IdentityGovernance.AccessReviews.Definitions.PostAsync(requestBody);


```
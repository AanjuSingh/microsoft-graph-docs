---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CreateReplyAllRequestBody
{
	Message = new 
	{
		Attachments = new List<Attachment>
		{
			new Attachment
			{
				@odata.type = "#microsoft.graph.fileAttachment",
				Name = "guidelines.txt",
				AdditionalData = new()
				{
					{"contentBytes", "bWFjIGFuZCBjaGVlc2UgdG9kYXk="},
				}
			},
		}
	},
	Comment = "if the project gets approved, please take a look at the attached guidelines before you decide on the name.",
};
var result = await graphClient.Me.Messages["message-id"].CreateReplyAll.PostAsync(requestBody);


```
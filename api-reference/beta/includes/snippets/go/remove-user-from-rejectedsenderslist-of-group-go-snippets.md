---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphgroups "github.com/microsoftgraph/msgraph-beta-sdk-go/groups"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



requestId := "https://graph.microsoft.com/beta/users/{id}"

requestParameters := &graphgroups.GroupItemRejectedSenders$refRequestBuilderDeleteQueryParameters{
	Id: &requestId,
}
configuration := &graphgroups.GroupItemRejectedSenders$refRequestBuilderDeleteRequestConfiguration{
	QueryParameters: requestParameters,
}

graphClient.Groups().ByGroupId("group-id").RejectedSenders().Ref().Delete(context.Background(), configuration)


```
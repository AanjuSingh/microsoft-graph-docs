---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphadmin "github.com/microsoftgraph/msgraph-beta-sdk-go/admin"
	  graphmodelswindowsupdates "github.com/microsoftgraph/msgraph-beta-sdk-go/models/windowsupdates"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphadmin.NewUpdateAudiencePostRequestBody()


updatableAsset := graphmodelswindowsupdates.NewUpdatableAsset()
id := "String (identifier)"
updatableAsset.SetId(&id) 

addMembers := []graphadmin.Objectable {
	updatableAsset,

}
requestBody.SetAddMembers(addMembers)

graphClient.Admin().Windows().Updates().DeploymentAudiences().ByDeploymentAudienceId("deploymentAudience-id").MicrosoftGraphWindowsUpdatesUpdateAudience().Post(context.Background(), requestBody, nil)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphsolutions "github.com/microsoftgraph/msgraph-beta-sdk-go/solutions"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphsolutions.NewGetPlanPostRequestBody()
target := graphmodels.NewBusinessScenarioTaskTargetBase()
taskTargetKind := graphmodels.GROUP_PLANNERTASKTARGETKIND 
target.SetTaskTargetKind(&taskTargetKind) 
additionalData := map[string]interface{}{
	"groupId" : "7a339254-4b2b-4410-b295-c890a16776ee", 
}
target.SetAdditionalData(additionalData)
requestBody.SetTarget(target)

result, err := graphClient.Solutions().BusinessScenarios().ByBusinessScenarioId("businessScenario-id").Planner().GetPlan().Post(context.Background(), requestBody, nil)


```
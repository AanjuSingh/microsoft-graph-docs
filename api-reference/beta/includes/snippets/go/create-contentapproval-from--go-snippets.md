---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodelswindowsupdates "github.com/microsoftgraph/msgraph-beta-sdk-go/models/windowsupdates"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodelswindowsupdates.NewComplianceChange()
additionalData := map[string]interface{}{
content := graphmodels.New()
catalogEntry := graphmodels.New()
id := "6b7e60db-a8e4-426a-9aed-bd12b5c0b9d4"
catalogEntry.SetId(&id) 
	content.SetCatalogEntry(catalogEntry)
	requestBody.SetContent(content)
deploymentSettings := graphmodels.New()
	requestBody.SetDeploymentSettings(deploymentSettings)
schedule := graphmodels.New()
startDateTime := "String (timestamp)"
schedule.SetStartDateTime(&startDateTime) 
gradualRollout := graphmodels.New()
endDateTime := "String (timestamp)"
gradualRollout.SetEndDateTime(&endDateTime) 
	schedule.SetGradualRollout(gradualRollout)
	requestBody.SetSchedule(schedule)
}
requestBody.SetAdditionalData(additionalData)

result, err := graphClient.Admin().Windows().Updates().UpdatePolicies().ByUpdatePolicieId("updatePolicy-id").ComplianceChanges().Post(context.Background(), requestBody, nil)


```
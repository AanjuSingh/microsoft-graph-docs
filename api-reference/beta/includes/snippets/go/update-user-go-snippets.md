---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/models"
	  //other-imports
)

graphClient, err := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewUser()
businessPhones := []string {
	"+1 425 555 0109",

}
requestBody.SetBusinessPhones(businessPhones)
officeLocation := "18/2111"
requestBody.SetOfficeLocation(&officeLocation) 

result, err := graphClient.Me().Patch(context.Background(), requestBody, nil)


```
---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-beta-sdk-go/Security/Cases/EdiscoveryCases/Item/Searches/Item/NoncustodialSources/Item"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewNoncustodialSource()
additionalData := map[string]interface{}{
	"odataId" : "https://graph.microsoft.com/beta/security/cases/ediscoveryCases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialDataSources/39333641443238353535383731453339", 
}
requestBody.SetAdditionalData(additionalData)

graphClient.Security().Cases().EdiscoveryCases().ByEdiscoveryCaseId("ediscoveryCase-id").Searches().BySearcheId("ediscoverySearch-id").NoncustodialSources().ByNoncustodialSourceId("ediscoveryNoncustodialDataSource-id").Post(context.Background(), requestBody, nil)


```
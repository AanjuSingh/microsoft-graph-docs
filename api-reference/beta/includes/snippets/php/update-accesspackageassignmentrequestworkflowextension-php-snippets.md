---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new AccessPackageCustomWorkflowExtension();
$additionalData = [
		'@odata.type' => '#microsoft.graph.accessPackageAssignmentRequestWorkflowExtension', 
		'displayName' => 'test_action_0124_email', 
		'description' => 'this is for graph testing only', 
];
$requestBody->setAdditionalData($additionalData);




$graphServiceClient->identityGovernance()->entitlementManagement()->accessPackageCatalogs()->byAccessPackageCatalogId('accessPackageCatalog-id')->accessPackageCustomWorkflowExtensions()->byAccessPackageCustomWorkflowExtensionId('customCalloutExtension-id')->put($requestBody);


```
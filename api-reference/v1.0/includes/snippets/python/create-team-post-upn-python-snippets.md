---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new Team();
$requestBody->setDisplayName('My Sample Team');

$requestBody->setDescription('My Sample Team’s Description');

$membersConversationMember1 = new ConversationMember();
$membersConversationMember1->set@odatatype('#microsoft.graph.aadUserConversationMember');

$membersConversationMember1->setRoles(['owner', ]);

$additionalData = [
'user@odata.bind' => 'https://graph.microsoft.com/v1.0/users(\'jacob@contoso.com\')', 
];
$membersConversationMember1->setAdditionalData($additionalData);



$membersArray []= $membersConversationMember1;
$requestBody->setMembers($membersArray);


$additionalData = [
'template@odata.bind' => 'https://graph.microsoft.com/v1.0/teamsTemplates(\'standard\')', 
];
$requestBody->setAdditionalData($additionalData);




$requestResult = $graphServiceClient->teams()->post($requestBody);


```
---
description: "Automatically generated file. DO NOT MODIFY"
---
<!-- markdownlint-disable MD041 -->

```java
GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ChatInfo chatInfo = new ChatInfo();
chatInfo.threadId = "19:7ebda77322dd4505ac4dedb5b67df076@thread.tacv2";

OffsetDateTime startDateTime = OffsetDateTimeSerializer.deserialize("2/5/2020 8:49:21 PM");

OffsetDateTime endDateTime = OffsetDateTimeSerializer.deserialize("2/5/2020 9:19:21 PM");

String externalId = "7eb8263f-d0e0-4149-bb1c-1f0476083c56";

MeetingParticipants participants = new MeetingParticipants();
LinkedList<MeetingParticipantInfo> attendeesList = new LinkedList<MeetingParticipantInfo>();
MeetingParticipantInfo attendees = new MeetingParticipantInfo();
IdentitySet identity = new IdentitySet();
Identity user = new Identity();
user.id = "1f35f2e6-9cab-44ad-8d5a-b74c14720000";
identity.user = user;
attendees.identity = identity;
attendees.upn = "test1@contoso.com";
attendeesList.add(attendees);
participants.attendees = attendeesList;

String subject = "Create a meeting with customId provided";

graphClient.me().onlineMeetings()
    .createOrGet(OnlineMeetingCreateOrGetParameterSet
        .newBuilder()
        .withChatInfo(chatInfo)
        .withEndDateTime(endDateTime)
        .withExternalId(externalId)
        .withParticipants(participants)
        .withStartDateTime(startDateTime)
        .withSubject(subject)
        .build())
    .buildRequest()
    .post();
```

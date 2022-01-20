---
title: "Working with Microsoft Teams messaging"
description: "Working with Microsoft Teams messaging"
author: "RamjotSingh"
ms.localizationpriority: high
ms.prod: "microsoft-teams"
ms.custom: scenarios:getting-started
---

# Working with Microsoft Teams messaging

Microsoft Teams has a comprehensive set of APIs for performing messaging operations on Microsoft Teams using Microsoft Graph. This document lists the various schema elements used by these APIs and makes suggestions on the APIs to use based on the scenario being targetted by the caller. The list of scenarios is in no way comprehensive but should guide the callers which API to invoke based on high level scenarios.

## Understanding chatMessage schema

[chatMessage](/graph/api/resources/chatMessage?preserve-view=true) represents messages in Microsoft Teams [chats](/graph/api/resources/chat?preserve-view=true) and [channels](/graph/api/resources/channel?preserve-view=true). In this section we will be describing various elements of the schema itself.

> **Note:** Examples shared below only show the relevant schema elements and not the entire message payload

### attachments

[Attachments](/graph/api/resources/chatmessageattachment?preserve-view=true) represents entities which can be referenced from a [chatMessage](/graph/api/resources/chatMessage?preserve-view=true). This includes objects like files, tabs, cards, meetings or other messages. The items themselves might be located somewhere else. For example, files might be stored in SharePoint. Section below describes various possibilities

#### file

When an [attachment](/graph/api/resources/chatmessageattachment?preserve-view=true) object refers to a file, it has information about the file including the link to open the file. The file itself is located in an accessible store like SharePoint. When refering to a file attachment, `contentType` is set to `reference`. Additionally, the file url is located in `contentUrl`.

> **Note:** The SharePoint url is link used to render the file, it is not the Microsoft Graph url. Callers can however use [Access shared items](/graph/api/shares-get?preserve-view=true) API to get the info and content of the file.

Example of an attachment with reference to a file

```json
    "attachments": [
        {
            "id": "924D1F74-E0D2-4927-8A67-15ECEF455527",
            "contentType": "reference",
            "contentUrl": "https://testing.sharepoint.com/sites/Samples/Shared Documents/General/color.png",
            "content": null,
            "name": "color.png",
            "thumbnailUrl": null
        }
    ],
```

#### tab

[Attachment](/graph/api/resources/chatmessageattachment?preserve-view=true) object refers to a [tab](/graph/api/resources/teamstab?preserve-view=true) hosted in the present context. This is often used to refer to newly added tab. When referring to a [tab](/graph/api/resources/teamstab?preserve-view=true), `contentType` is set to `tabReference`, and `id` is set to the Id of the tab. Additionally, name is set to the provided name of the [tab](/graph/api/resources/teamstab?preserve-view=true).

Example of an attachment with reference to a tab

``` json
"attachments": [
        {
            "id": "tab::d64ea8d0-8b63-4f53-9bf6-806648176968",
            "contentType": "tabReference",
            "contentUrl": null,
            "content": null,
            "name": "Bing",
            "thumbnailUrl": null
        }
    ],
```
#### card

Cards represent visual elements backed by a pre-defined schema. Microsoft Teams supports various cards [as defined by Bot Framework](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object). Additionally, Microsoft Teams supports 2 additional cards

- Code snippet - With `contentType` set to `application/vnd.microsoft.card.codesnippet`
- Annoucement card - With `contentType` set to `application/vnd.microsoft.card.announcement`

For cards `contentType` is set to the type of card, while `content` itself represents the serialized json for the card.

> **Note:** Additionaly aspects of cards like images might refer to external resources of resources hosted by Microsoft Teams as [chatMessageHostedContent](/graph/api/resources/chatmessagehostedcontent?preserve-view=true).

Example of an attachment with adaptive card in it. This card has images in it hosted by Microsoft Teams

```json
    "attachments": [
        {
            "id": "74d20c7f34aa4a7fb74e2b30004247c5",
            "contentType": "application/vnd.microsoft.card.adaptive",
            "contentUrl": null,
            "content": "{  \"type\": \"AdaptiveCard\",  \"body\": [    {      \"items\": [        {          \"columns\": [            {              \"width\": \"auto\",              \"items\": [                {                  \"size\": \"medium\",                  \"url\": \"https://graph.microsoft.com/beta/teams/68a3e365-f7d9-4a56-b499-24332a9cc572/channels/19:0b50940236084d258c97b21bd01917b0@thread.skype/messages/1596694346004/hostedContents/aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQyLTUxZDYxNGE5MDQ5ZTU4MjFlMTRmMGI2NmExNmVlNzhlL3ZpZXdzL2ltZ28=/$value\",                  \"height\": \"auto\",                  \"type\": \"Image\"                },                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"SHADES\",                  \"weight\": \"bolder\",                  \"type\": \"TextBlock\"                }              ],              \"type\": \"Column\"            },            {              \"width\": \"stretch\",              \"items\": [                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"08/31/2019 19:30:00\",                  \"type\": \"TextBlock\"                },                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"Final\",                  \"spacing\": \"None\",                  \"type\": \"TextBlock\"                },                {                  \"horizontalAlignment\": \"center\",                  \"size\": \"extraLarge\",                  \"text\": \"40 - 7\",                  \"type\": \"TextBlock\"                }              ],              \"spacing\": \"Medium\",              \"separator\": true,              \"type\": \"Column\"            },            {              \"width\": \"auto\",              \"items\": [                {                  \"horizontalAlignment\": \"center\",                  \"size\": \"medium\",                  \"url\": \"https://graph.microsoft.com/beta/teams/68a3e365-f7d9-4a56-b499-24332a9cc572/channels/19:0b50940236084d258c97b21bd01917b0@thread.skype/messages/1596694346004/hostedContents/aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQyLWM4NjgwMjMzMzcyMzc2MmQ0MWEyY2QxMGVhMWI4ZGRhL3ZpZXdzL2ltZ28=/$value\",                  \"height\": \"auto\",                  \"type\": \"Image\"                },                {                  \"horizontalAlignment\": \"center\",                  \"text\": \"SKINS\",                  \"weight\": \"bolder\",                  \"type\": \"TextBlock\"                }              ],              \"spacing\": \"Medium\",              \"separator\": true,              \"type\": \"Column\"            }          ],          \"type\": \"ColumnSet\"        }      ],      \"type\": \"Container\"    }  ],  \"speak\": \"The Seattle Seahawks beat the Carolina Panthers 40-7\",  \"$schema\": \"http://adaptivecards.io/schemas/adaptive-card.json\",  \"version\": \"1.2\"}",
            "name": null,
            "thumbnailUrl": null
        }
    ]
```

#### meeting

When a meeting is scheduled in a channel, a message with meeting details is posted in the channel. A meeting attachment represents this object along with details of the meeting. `id` represents Id of the meeting, while `content` has details regarding organizer of the meeting and Exchange Id of the meeting. This Id can be used to look the meeting up using calendar APIs. `contentType` is set to `meetingReference` for meeting attachments.

Example of an attachment with meeting reference in it

```json
    "attachments": [
        {
            "id": "1628156567881",
            "contentType": "meetingReference",
            "contentUrl": null,
            "content": "{\"exchangeId\":\"AAMkAGU2NzgzNDQ3LWFkMTctNGY2MC05ZjM1LWFkOTYxZWZhYTY2MgBGAAAAAADFwPNVvpzXRqmCO5F6qAKtBwB89fWKTP8MSaPLNsJWtozvAAAAAAENAAB89fWKTP8MSaPLNsJWtozvAAFg-8IoAAA=\",\"organizerId\":\"8ea0e38b-efb3-4757-924a-5f94061cf8c2\"}",
            "name": "Testing channel meeting",
            "thumbnailUrl": null
        }
    ],
```

#### message

Attachment object refers to a message when a specific message is being replied to in a [chat](/graph/api/resources/chat?preserve-view=true). For message attachments, `id` represents Id of the message. `content` contains additional details for example preview text of the message and sender of the message being replied to. `contentType` is set to `messageReference` for such attachments.

Example of an attachment with message reference in it

```json
    "attachments": [
        {
            "id": "1622853091207",
            "contentType": "messageReference",
            "contentUrl": null,
            "content": "{\"messageId\":\"1622853091207\",\"messagePreview\":\"Testing unread read status\",\"messageSender\":{\"application\":null,\"device\":null,\"user\":{\"userIdentityType\":\"aadUser\",\"id\":\"8ea0e38b-efb3-4757-924a-5f94061cf8c2\",\"displayName\":\"Alex\"}}}",
            "name": null,
            "thumbnailUrl": null
        }
    ],
```

### body

`body` represents the body of the message. `body` in itself can refer to other elements in the schema like mentions, attachments. Body can be `text` or `html` as represented by the `contentType` property.

Microsoft Teams supports additional schema elements which are outside of the HTML specifications to support additional elements like mentions. Following elements are supported by `chatMessage` schema which are not HTML elements

- at - Reference to an [chatMessageMention](/graph/api/resources/chatmessagemention?preserve-view=true) representing details of a user, application, [channel](/graph/api/resources/channel?preserve-view=true), [team](/graph/api/resources/team?preserve-view=true) or [tag](/graph/api/resources/teamworktag?preserve-view=true) being @mentioned
- attachment - Representing the position of an attachment reference
- systemEventMessage - When body `content` is set to `<systemEventMessage/>`, it means the message represents a special event. You can read more about system events [here](/graph/system-messages).

#### Example of a message with @mention for a team

```json
    "body": {
        "contentType": "html",
        "content": "<div><div><at id=\"0\">WebhookTesting</at>&nbsp;Hello team</div></div>"
    },
    "mentions": [
        {
            "id": 0,
            "mentionText": "WebhookTesting",
            "mentioned": {
                "application": null,
                "device": null,
                "user": null,
                "tag": null,
                "conversation": {
                    "id": "68a3e365-f7d9-4a56-b499-24332a9cc572",
                    "displayName": "WebhookTesting",
                    "conversationIdentityType": "team"
                }
            }
        }
    ],
```

#### Example of a message with attachment

```json
    "body": {
        "contentType": "html",
        "content": "Scheduled a meeting<attachment id=\"1628156567881\"></attachment>"
    },
    "attachments": [
        {
            "id": "1628156567881",
            "contentType": "meetingReference",
            "contentUrl": null,
            "content": "{\"exchangeId\":\"AAMkAGU2NzgzNDQ3LWFkMTctNGY2MC05ZjM1LWFkOTYxZWZhYTY2MgBGAAAAAADFwPNVvpzXRqmCO5F6qAKtBwB89fWKTP8MSaPLNsJWtozvAAAAAAENAAB89fWKTP8MSaPLNsJWtozvAAFg-8IoAAA=\",\"organizerId\":\"8ea0e38b-efb3-4757-924a-5f94061cf8c2\"}",
            "name": "Testing channel meeting",
            "thumbnailUrl": null
        }
    ],
```

#### Example of a message with system event in it

```json
    "body": {
        "contentType": "html",
        "content": "<systemEventMessage/>"
    },
    "channelIdentity": {
        "teamId": "68a3e365-f7d9-4a56-b499-24332a9cc572",
        "channelId": "19:0b50940236084d258c97b21bd01917b0@thread.skype"
    },
    "attachments": [],
    "mentions": [],
    "reactions": [],
    "eventDetail": {
        "@odata.type": "#microsoft.graph.conversationMemberRoleUpdatedEventMessageDetail",
        "conversationMemberRoles": [],
        "conversationMemberUser": {
            "id": "c4aefc8e-f890-4aa6-b586-6cce899ff7f8",
            "displayName": null,
            "userIdentityType": "aadUser"
        },
        "initiator": {
            "application": null,
            "device": null,
            "user": {
                "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                "displayName": null,
                "userIdentityType": "aadUser"
            }
        }
    }
```

### channelIdentity

If [chatMessage](/graph/api/resources/chatmessage?preserve-view=true) was sent in a [channel](/graph/api/resources/channel?preserve-view=true), `channelIdentity` represents the details about the channel. This includes Id of the [channel](/graph/api/resources/channel?preserve-view=true) and Id of the [team](/graph/api/resources/team?preserve-view=true). This property is read-only.

Example of `channelIdentity` in a message

```json
    "channelIdentity": {
        "teamId": "68a3e365-f7d9-4a56-b499-24332a9cc572",
        "channelId": "19:0b50940236084d258c97b21bd01917b0@thread.skype"
    },
```

### chatId

If [chatMessage](/graph/api/resources/chatmessage?preserve-view=true) was sent in a [chat](/graph/api/resources/chat?preserve-view=true), `chatId` represents the Id of the chat in which message was sent. This property is read-only.

Example of `chatId` in a message

```json
"chatId": "19:8ea0e38b-efb3-4757-924a-5f94061cf8c2_976f4b31-fd01-4e0b-9178-29cc40c14438@unq.gbl.spaces",
```

### createdDateTime

`createdDateTime` represents the time when the message was created on the server. This timestamp might be different than when the message was sent by the caller. Server records only server side timestamp. This property is usually read-only, however it can be written when [importing messages from an external system](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).

### deletedDateTime

If [chatMessage](/graph/api/resources/chatmessage?preserve-view=true) was deleted, `deletedDateTime` represents the time of deletion for the message. This property is read-only.

> **Note:** Deleted messages are not always returned by all the APIs. [Change notifications](/graph/teams-changenotifications-chatmessage) always return deleted message notifications if subscription include deleted change type.

### etag

`etag` represents the version of the message. Any changes to message (including reactions, edits etc) change the `etag` of the message. This property is read-only.

### eventDetail

If present, represents details of an event that happened in a [chat](/graph/api/resources/chat?preserve-view=true), a [channel](/graph/api/resources/channel?preserve-view=true), or a [team](/graph/api/resources/team?preserve-view=true), for example, adding new members. For event messages, the messageType property will be set to `systemEventMessage`. You can read more about system events [here](/graph/system-messages).

### from

Represents the sender of the message. Microsoft Teams supports a large set of senders

- Azure AD users - Users who have a valid Azure AD user. This includes [Azure AD guests](/azure/active-directory/external-identities/what-is-b2b) and [native federation](/microsoftteams/manage-external-access)

    Following example shows the `from` element for a message sent by Azure AD user
    ```json
    "from": {
        "application": null,
        "device": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Alex Wilber",
            "userIdentityType": "aadUser"
        }
    },
    ```
- Anonymous guests - Users who join a meeting using join link. These users provide a display name when joining meeting. They have no persistent identity in Microsoft 365.
    
    Following example shows the `from` element for a message sent by an anonymous guest
    ```json
    "from": {
        "application": null,
        "device": null,
        "user": {
            "id": "8578568e393e4ffe8763e0b7c3da01fe",
            "displayName": "Anon (Guest)",
            "userIdentityType": "anonymousGuest"
        }
    },
    ```

- Personal Microsoft account users - Users using their personal Microsoft account to login into Microsoft Teams

    Following example shows the `from` element for a message sent by anonymous guest

    ```json
    "from": {
        "application": null,
        "device": null,
        "user": {
            "id": "d78f5bc88c39f6b8",
            "displayName": "TFL 1017",
            "userIdentityType": "personalMicrosoftAccountUser"
        }
    },
    ```
- Skype users - Skype (for consumer) users. You can learn more about this interop [here](/microsoftteams/teams-skype-interop)
    
    Following example shows the `from` element for a message sent by anonymous guest

    ```json
    "from": {
        "application": null,
        "device": null,
        "user": {
            "id": "alex1122",
            "displayName": "Alex",
            "userIdentityType": "skypeUser"
        }
    },
    ```
- Skype for business onpremise users - Users using Skype For Business onpremise offering. You learn more about this [here](/microsoftteams/teams-and-skypeforbusiness-coexistence-and-interoperability)

     Following example shows the `from` element for a message sent by anonymous guest

    ```json
    "from": {
        "application": null,
        "device": null,
        "user": {
            "id": "b0eddfe2-659b-437d-b289-cf55c8b3bb1d",
            "displayName": "Alex",
            "userIdentityType": "onPremiseAadUser"
        }
    },
    ```
- Bots - Bots using [Microsoft Bot Framework](/azure/bot-service/?view=azure-bot-service-4.0) to write conversational bots

    Following example shows the `from` element for a message sent by bot

    ```json
    "from": {
        "device": null,
        "user": null,
        "application": {
            "id": "358f0194-6b0e-4dd3-af35-c24fe8a9ec87",
            "displayName": "Flow",
            "applicationIdentityType": "bot"
        }
    }
    ```
- Outgoing webhooks - Outgoing webhooks allow developers to build a low cost solution which is in some respects similar to bots. You can read more about outgoing webhooks [here](/microsoftteams/platform/webhooks-and-connectors/how-to/add-outgoing-webhook)

    Following example shows the `from` element for a message sent by bot

    ```json
    "from": {
        "device": null,
        "user": null,
        "application": {
            "id": "22e50a9b-80cc-4eab-a092-ce64796d28d7",
            "displayName": "Custom bot",
            "applicationIdentityType": "outgoingWebhook"
        }
    }
    ```
- Office 365 connectors - Office 365 connectors allow posting one way messages to Microsoft Teams. You can learn more about this integration [here](/microsoftteams/platform/webhooks-and-connectors/how-to/connectors-creating)
    
    Following example shows the `from` element for a message from Office 365 connector

    ```json
    "from": {
        "device": null,
        "user": null,
        "application": {
            "id": "4c6cfc6e-cf78-44e8-87fd-bbb0efcad6a2",
            "displayName": "Bing News",
            "applicationIdentityType": "office365Connector"
        }
    }
    ```

This property is usually read-only, however it can be written when [importing messages from an external system](/microsoftteams/platform/graph-api/import-messages/import-external-messages-to-teams).

> **Note:** Display name isn't always present

### id

Unique Id representing the message. This property is read-only.

> **Note:** Id is unique only under a specific scope i.e. chat or a channel. Different messages across chats and channels might have same Id.

### importance

Represents importance of the message. Possible values are

- normal
- high
- urgent

Example of a message with importance set to high

```json
"importance": "high",
```

### lastEditedDateTime

Represents the timestamp when the message was edited by the user. This is represented in Microsoft Teams UI with `Edited` flag.

### lastModifiedDateTime

Represents the timestamp when the message was last modified. This includes changes like reactions. `eTag` and `lastModifiedDateTime` both change together.

### mentions

Represents users, applications (bots, webhooks etc), channels, teams or tags being @mentioned.

#### Example of a message with @mention for another user

```json
    "body": {
        "contentType": "html",
        "content": "<div><div><div><div><at id=\"0\">Alex</at>&nbsp;Test123</div></div></div></div>"
    },
    "mentions": [
        {
            "id": 0,
            "mentionText": "Alex",
            "mentioned": {
                "application": null,
                "device": null,
                "conversation": null,
                "tag": null,
                "user": {
                    "id": "c27c1b19-3904-4822-9813-4f6bdaab2eae",
                    "displayName": "Alex",
                    "userIdentityType": "aadUser"
                }
            }
        }
    ],
```

#### Example of a message with @mention for a bot

```json
    "body": {
        "contentType": "html",
        "content": "<div><div><at id=\"0\">Power Automate</at> Learn more&nbsp;</div></div>"
    },
    "mentions": [
        {
            "id": 0,
            "mentionText": "Power Automate",
            "mentioned": {
                "device": null,
                "user": null,
                "conversation": null,
                "tag": null,
                "application": {
                    "id": "358f0194-6b0e-4dd3-af35-c24fe8a9ec87",
                    "displayName": "Power Automate",
                    "applicationIdentityType": "bot"
                }
            }
        }
    ],
```

#### Example of a message with @mention for a team

```json
    "body": {
        "contentType": "html",
        "content": "<div><div><at id=\"0\">WebhookTesting</at>&nbsp;Hello team</div></div>"
    },
    "mentions": [
        {
            "id": 0,
            "mentionText": "WebhookTesting",
            "mentioned": {
                "application": null,
                "device": null,
                "user": null,
                "tag": null,
                "conversation": {
                    "id": "68a3e365-f7d9-4a56-b499-24332a9cc572",
                    "displayName": "WebhookTesting",
                    "conversationIdentityType": "team"
                }
            }
        }
    ],
```

### messageType

Represents the type of message. The values in use are 

- message - Representing messages sent by users, applications etc
- systemEventMessage - Represents messages sent by Microsoft Teams with details about various events like adding members, deleting channels etc. You can read more about system events [here](/graph/system-messages).

Additional values not used right now

- typing
- chatEvent

### onBehalfOf

User attribution of the message when bot sends a message on behalf of a user. You can read more about user attribution [here](/microsoftteams/platform/messaging-extensions/how-to/action-commands/respond-to-task-module-submit?tabs=dotnet%2Cdotnet-1#user-attribution-for-bots-messages).

Example of a message sent by a bot on behalf of a user

```json
"from": {
        "device": null,
        "user": null,
        "application": {
            "id": "8a34cb8d-65dc-44e2-8375-a2261d1f2a4b",
            "displayName": "PolicyMaker",
            "applicationIdentityType": "bot"
        }
    },
    "onBehalfOf": {
        "application": null,
        "device": null,
        "user": {
            "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
            "displayName": "Alex Wilber",
            "userIdentityType": "aadUser"
        }
    },
```

### policyViolation

If the message violated any data loss prevention (DLP) policies set by the tenant, a message PATCH can be invoked with the details of the policy being violated. This hides the message from the Microsoft Teams UI. This element represents the details of the policy being violated, along with the action.

Example of a message blocked due to policy

```json
    "body": {
        "contentType": "text",
        "content": ""
    },
    "policyViolation": {
        "dlpAction": "blockAccess",
        "justificationText": null,
        "userAction": "none",
        "verdictDetails": "none",
        "policyTip": null
    },
```

### reactions

Represents reactions from other users on this message. This includes reactions like likes etc. Each elements represents information about the reaction and the user who reacted.

Example of a message with reaction in it

```json
    "reactions": [
        {
            "reactionType": "like",
            "createdDateTime": "2022-01-18T23:41:57.573Z",
            "user": {
                "application": null,
                "device": null,
                "user": {
                    "id": "8ea0e38b-efb3-4757-924a-5f94061cf8c2",
                    "displayName": null,
                    "userIdentityType": "aadUser"
                }
            }
        }
    ]
```

> **Note:** Display name isn't always present

### replyToId

Represents the Id of the message this message is a reply to in a reply chain. This property is only set for channel messages. This property is read-only.

> **Note:** For replying to messages in a chat, message reference is used. Additionally, chats allowing multiple of message reference elements.

### subject

Subject of the message. This is valid only for messages sent in channel.

### webUrl

Url pointing to the message in Microsoft Teams UI. This url can be used to open the message directly in Microsoft Teams UI in a browser.

## Choosing the right API for your scenarios

Choosing the right API is essential for getting the best experience. Additionally, using the right set of APIs will allow you to fetch data without hitting throttling.

Messaging APIs in Microsoft Teams are divided in 3 major categories

- APIs focused on the way Microsoft Teams UI works. Any changes are instantly visible
- Slow sync APIs focused on users and teams. Any changes can take up to 24 hours to be available
- Change notifications based APIs to get notified in real time

### Microsoft Teams UI aligned APIs

These APIs allow you to get older methods similar to how Microsoft Teams UI does. These APIs are built to allow 'once in a while' sync to get messages in a specific context. These APIs are highly performant and any changes (messages sent, edited or deleted) are instantly visible through these APIs.

Following APIs belong to this set

- [List messages in a chat](/graph/api/chat-list-messages?preserve-view=true)
- [List messages in a channel](/graph/api/channel-list-messages?preserve-view=true)
- [List replies to a message in a channel](/graph/api/chatmessage-list-replies?preserve-view=true)
- [Send message in a chat](/graph/api/chat-post-messages?preserve-view=true)
- [Send message in a channel](/graph/api/chatmessage-post?preserve-view=true)
- [Reply to a message in a channel](/graph/api/chatmessage-post-replies?preserve-view=true)
- [List hostedContents associated with a message](/graph/api/chatmessage-list-hostedcontents?preserve-view=true)
- [Get hostedContent associated with a message](/graph/api/chatmessagehostedcontent-get?preserve-view=true)

Additionally, following APIs act along with the APIs above to serve specific scenarios regarding fetching specific instances or changing order of traversal

- [Get a message or reply in a channel or a chat](/graph/api/chatmessage-get?preserve-view=true)
- [Continuous sync using /delta for channel messages](/graph/api/chatmessage-delta?preserve-view=true)

### APIs for exporting data from Microsoft Teams

These APIs typically work at a higher granularity than UI aligned APIs. These APIs focus on allowing fetching large amount of data. It might take a while (upto 24 hours in certain cases) for data to get synced and being available through these APIs.

- [List messages across a user's chats](/graph/api/chats-getallmessages?preserve-view=true)
- [List messages across channels in a team](/graph/api/channel-getallmessages?preserve-view=true)

### Realtime APIs

Realtime APIs allow caller to get notified as soon as a change is made (message sent, edited, deleted etc). These APIs are suitable for realtime applications like rendering messages outside of Microsoft Teams UI. Additionally, these APIs allow creating subscriptions and thus allow receving large amount of data without hitting throttling. Refer to [this](/graph/teams-changenotifications-chatmessage) document for more details.


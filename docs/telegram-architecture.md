## Product choice

Telegram messenger
Link[https://web.telegram.org]
Telegram is a messenger, allowing connection from multiple platforms, such as mobile, desktop and web.

## Main components

![Telegram Component Diagram](diagrams/out/telegram/component-diagram/Component%20Diagram.svg)

[Telegram Component Diagram PlantUML](diagrams/src/telegram/component-diagram.puml)

* Mobile app - connects to the connection layer and acts as a data sender and reciever.
* 3rd party bot services - allow the functionality of any external bots via connection to the telegram bot API server
* SMS providers - allow the 2FA to work via SMS messages with one-time use codes.
* Message handling service - handles all the interactions of messages with servers.
* AUTH & Session service - handles the account access and verification.

## Data flow

![Telegram Sequence Diagram](diagrams/out/telegram/sequence-diagram/Sequence%20Diagram.svg)

[Telegram Sequence Diagram PlantUML](diagrams/src/telegram/sequence-diagram.puml)

Event propagation via mobile software.

It has 3 possible actions:

1. Publish event (NewMessageUpdate). It connects to the Kafka event bus, notifying it about recieving a new message.
2. Consume (sync to online devices). It collects any possible new data from the Kafka event bus while the app is idle in the background.
3. Update UI per tick, getting the data from the connection layer (i.e. new messages, edits, etc).

## Deployment

![Telegram Deployment Diagram](diagrams/out/telegram/deployment-diagram/Deployment%20Diagram.svg)

[Telegram Deployment Diagram PlantUML](diagrams/src/telegram/deployment-diagram.puml)

The components are deployed in the servers. The messages and media are in the storage clusters.

## Assumptions

I assume the cloud storage system implements deduplication to optimize storage costs for shared media files.
I assume the messenger uses deeper encryption systems, not described in diagrams.

## Open questions

How does the data flow look like in secret chats?
How does the data encryption flow look like in terms of all messages?
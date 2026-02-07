## Product Choice

Provide:

    Product name;
    Link to the product's website;
    Short description of the product (1-2 sentences).

## Main components

![WildBerries Component Diagram](diagrams/out/wildberries/architecture-component/Component%20Diagram.svg)

[Wildberries Component Diagram code](diagrams/src/wildberries/architecture-component.puml)

#### PVZ software
This component is to engage WildBebris workers during breaks. An exciting day it is when one plays Plants versus Zombies!

#### Customer mobile app
This is the bloated app we have to download from the Play store to buy labubas

#### SMS service
This is obviously to get users to pay for sms codes sent to them or else send them from MAX

#### Auth service
A service to keep users logged in and not ask them their password and email every visit like moodle does

#### Logistics and Routing
This is used to get your parcel delievered to you from Kazan to Innopolis

## Data flow
![WildBerries Sequence Diagram](diagrams/out/wildberries/architecture-sequence/Sequence%20Diagram.svg)
In prep stage user clicks an "Add to cart" button in the Mobile app / Browser and it sends an RTC addToCart request to gateway which in turn updates session cart in the service and then does redis hot data black magic which then returns OK. After that we simply return 2 times and update ui.

## Deployement
![WildBerries Deployment Diagram](diagrams/out/wildberries/architecture-deployment/Deployment%20Diagram.svg)

[Wildberries Component Diagram code](diagrams/src/wildberries/architecture-deployment.puml)

Sooo components live in user's phones, their partner's phones, enterprise hardware and in global infrastructure.

## Assumptions
1. I assume the prices never go down because sales aren't real 💯
2. I assume that it is expensive to pull data from caches, that is why the implementation includes hot cache thingy

## Open questions
1. What even is this
2. How do warehouses operate
3. What is an event bus
4. What is a gateway

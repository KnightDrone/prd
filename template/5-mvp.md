# The MVP

## Personas and Scenarios
The WildKnight MVP aims to provide a service that enhances the wellbeing and convenience of outdoor adventures by providing essential supplies via drone delivery to remote locations. The target personas for this product are outdoor enthusiasts, hikers, and campers who enjoy exploring remote areas. The key persona is the outdoor enthusiast who values convenience and safety during their adventures.

*Who are the target personas for this product?*

*Which is the key persona?*

*High-level scenarios to adopt, use and share the product.*

## User Stories and Key Features
### User stories for hikers
- As a hiker, I would like to see where I am on the map before placing an order.
- As a hiker. I would like to see the selection of items available for order before choosing.
- As a hiker, I would like to have offline guides with tips for hiking.
- As a hiker, I would like to get hiking tips from a chatbot.
- As a hiker, I would like to see how long until my order arrives.
- As a hiker, I would like to download parts of the map.

### User stories for operators
- As an operator, I would like to filter pending orders.
- As an operator, I would like to see the pending orders marked on the map.
- As an operator, I would like the ability to accept or reject order requests.

### Key features
- **Map**: This is essential in a delivery app, for both hikers and operators. For hikers it can be handy to see where they are in the wilderness, as well as serving as a reminder for where their order will be delivered. For operators it is imperative that they see where they are delivering items to, and allows them to decide whether a hiker is too far for delivery. In addition, parts of the map can be downloaded for offline use.
- **Order Menu**: A clean menu for hikers to select what they need, provides additional information on each item plus their price. A hiker with a scratch would not want to browse for items, so we kept the screen very minimal.
- **Pending Orders**: Operators need to see what orders are available, when they were placed, where from, and what item was ordered. We give the operator the option to filter the orders, perhaps an operator only has one item in stock, or only delivers to a certain location.
- **Offline Guides**: A very helpful offline feature is the guides. They are accessible with or without auth and can provide useful tips to new hikers.

*User stories about how various personas will use the product in context.*

*Identify and prioritise the key features required.*

*Justify the importance of each feature.*

## Success Criteria
Around 2.7 million people identify as active hikers in Switzerland according to survey from 2017. We can assume the number has increased with a general increase in population. A target for us is to capture 1% of that market in the first 3 months, so around 30,000 users. Along with this, we would like to see 1000 operators, this could be marketed as a "side hustle" for people looking to make some extra money on the side. For hiking, an activity mostly done on weekends, DAU does not make sense as a metric for us as usage will be very unevenly distributed. Instead we will measure WAU (weekly active users) and hope to acheive 5% WAU (500 users) as well as 50% MAU (5,000 users). On the operator side, we are targeting a WAU of 20% (200 operators), and MAU of 75% (750 operators). 

As for user statisfaction, we are targeting atleast 4 out of 5 rating on the app store within our first 3 months. Along with reviews we will measure feedback through online communication, such as through forums and other social channels. For the operators, it will be imperative that we communicate with them in person to gather feedback on their side as without operators we have no product.

*How will you evaluate the success of the MVP?*

*Metrics include user penetration, quality / satisfaction.*

*If applicable, progress in discussions with ecosystem partners / investors / customers.*

## Features Outside the Scope

Our MVP does not have autonomous drone delivery, which was part of the initial pitch. This is due to the technical difficulty it provided, and was not absolutely necessary for a successful MVP in which a buyer orders an item and gets it delivered by drone. Our long-term goal is to integrate DJI API to allow for autonomous drone delivery. Relying on operators is a temporary fix as ideally we would have our own drone fleet and supplies that would be managed autonomously. This would allow the number of users that can be served to not be limited by how many operators are online or what supply they have. In addition, this would increase throughput of delivery as the more efficient path-finding algorithm would be built in to these drones. An intermediate step would be a directions interface for the operators that shows them the quickest path to the buyer.  

*The MVP must be viable and minimal.*

*Which features don’t belong in it.*

*How should these be eventually integrated and in what sequence.*


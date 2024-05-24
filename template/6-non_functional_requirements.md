# Non-Functional Requirements

## Security, privacy, and data retention policies

### Data and Privacy
All authentication is handled by Google firebase, we do not store sensitive information like passwords in our databases. What we do store is limited information about the user necessary to identify them as well as information on orders such as location, date, item ordered. 

### Laws and Regulations
Since we are using drones, we have to be very careful with legal considerations. This will be a major part of our communication with operators. We will only allow certain drones to be used, since drones that weigh less than 250g do not require training to fly in Switzerland. In addition, drone operators will have to provide proof of identity as they must be over the age of 18. We will be careful not to allow orders from locations where drones are not allowed to fly, for example near air fields, penal institutions, and nuclear power plants. Since this app is for hikers it is unlikely this safeguard will be used but it is crucial to have in place.
*Which are the applicable laws and regulations?*

*What are your internal policies?*

*Which privacy features do you need from the phone?*

## Adoptions, Scalability and Availability
We will initially keep fees relatively low to drive early adoptions as well as give bonuses to early operators. It is just as important to get operators on board as well as hikers looking to purchase items.

We expect traffic to be quite uneven. It will most likely be low during the week and much more busy during the weekend. We expect little to no traffic at night time. Since we are using firebase for our backend, the scalability and availability of services will be handled for us

*What kind of traffic patterns do you expect to see?*

*Are there known periods of bursty traffic that the MVP must be designed to support?*


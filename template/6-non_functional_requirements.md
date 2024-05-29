# Non-Functional Requirements

## Security, privacy, and data retention policies

### Data and privacy
All authentication is handled by Google firebase, we do not store sensitive information like passwords in our databases. In terms of user data, within our Firestore database we store the user's account creation date, name, email, and role as well as all the orders they have partaken in, either as a buyer or as an operator. Location data is read locally and is never sent to our servers. We do not store any payment information, as all transactions are handled by Google Pay. We do not store any chatbot messages, as they are cached locally and not stored on our servers. The only privacy feature required from the phone is the user's location, this is necessary for the app to function as it is a delivery app.

### Laws and regulations
Since we are using drones, we have to be very careful with legal considerations. This will be a major part of our communication with operators. We will only allow certain drones to be used, since drones that weigh less than 250g do not require training to fly in Switzerland. In addition, drone operators will have to provide proof of identity as they must be over the age of 18. We will be careful not to allow orders from locations where drones are not allowed to fly, for example near air fields, penal institutions, and nuclear power plants. Since this app is for hikers it is unlikely this safeguard will be used but it is crucial to have in place.

## Adoptions, Scalability and Availability
We will initially keep fees relatively low to drive early adoptions as well as give bonuses to early operators. It is just as important to get operators on board as well as hikers looking to purchase items.

We expect traffic to be quite uneven. It will most likely be low during the week and much more busy during the weekend. We expect little to no traffic at night time. Since we are using firebase for our backend, the scalability and availability of services will be handled for us.


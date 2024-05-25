# Design and Implementation

## Frontend

*List the key libraries, languages, components used by the MVP.*

*If applicable, describe essential screens.*

## Backend

*Decompose the MVP into functional blocks.*

## Data Model
### Database
We are using the firestore database to store our data. We have two main collections, users and orders, which may be split across different geographical regions (perhaps cantons), however that is beyond the scope of even the MVP. 

#### Orders
Stores information about individual orders, this allows both hikers and operators to have access to order information.
Fields:
- Order ID (primary key)
- price
- operator start location
- operator ID
- operator name
- order date and time
- status (accepted, pending, cancelled, delivered)
- user ID
- order location
- delivery date and time

#### Users
Stores information on users to verify which pages and features they have access to. We do not store passwords in our database.
Fields:
- User ID (primary key)
- account creation date
- email
- username
- role (either user or operator)

### Other data
We also cache other data, but do not have access to it in our database. The data we cache is any map area users choose to download in addition to chats between users and the chat bot (until they clear message history).

*What data are you collecting / managing?*

*How is it organised?*

*Where is it stored?*

*How is it shared/copied/cached?*

## Security Considerations

## Infrastructure and Deployment

*How is the application developed, tested and deployed?*

*Any special infrastructure requirements.*

## Test Plan

*How is the application developed, tested and deployed?*

*Any special infrastructure requirements.*


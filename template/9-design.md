# Design and Implementation

## Frontend

### Key languages and libraries
FOr the development of our app, we used Typescript and React Native, which allows us to create a natively rendered mobile app that can be deployed to both Android and iOS. Despite our POC being focused and tested on Android, for our MVP we plan on rolling out to iOS and having the same codebase be deployable to both is a huge advantage. Along with this, React Native's fast performance and vast ecosystem of libraries made it very appealing to us. We used Typescript instead of Javascript due to the efficiency added by having static typing. This saved a lot of time while debugging and overall made the code much more readable. For the frontend design, we used Tailwind CSS, which allowed for consistent styling across the app. Moreover, we used Expo Go during development, this acccelerated our testing processes as it made running tests simple as well as giving us the ability to see changes to the code live on our phones. The modularity of React Native with its reusable components and Tailwind's utility-first approach give us a very scalable codebase that facilitates easy redesign and updates. 

### Essential screens
#### User screens
**login/signup screen**
This is the initial screen that loads (unless the user is already signed in)
Some essential screens include our login/signup page, the map, the order menu, the offline guides, and expected time of delivery for hikers. For operators there is the operator map, the pending orders screen, and the delivery accepted screen.

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


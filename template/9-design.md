# Design and Implementation

## Frontend

### Key languages and libraries
FOr the development of our app, we used Typescript and React Native, which allows us to create a natively rendered mobile app that can be deployed to both Android and iOS. Despite our POC being focused and tested on Android, for our MVP we plan on rolling out to iOS and having the same codebase be deployable to both is a huge advantage. Along with this, React Native's fast performance and vast ecosystem of libraries made it very appealing to us. We used Typescript instead of Javascript due to the efficiency added by having static typing. This saved a lot of time while debugging and overall made the code much more readable. For the frontend design, we used Tailwind CSS, which allowed for consistent styling across the app. Moreover, we used Expo Go during development, this acccelerated our testing processes as it made running tests simple as well as giving us the ability to see changes to the code live on our phones. The modularity of React Native with its reusable components and Tailwind's utility-first approach give us a very scalable codebase that facilitates easy redesign and updates. 

### Essential screens
#### User screens
- **Login/signup screen**: This is the initial screen that loads (unless the user is already signed in). It includes options for logging in with email or Google; a sign up page with fields for username, email, password, and confirmation; password recovery. The user interface is clean and straightforward, with clear instructions and error handling.
- **Map**: Logging in redirects here but if the user is already signed in, this is the initial screen. We use the Google Maps API to display the user's current location and nearby places of interest. The map has real-time location tracking and intuitive map controls with zoom in/out and a recenter button.
- **Order menu**: This is a simple menu that displays all items available. On clicking each card it displays the description, price, image of the item, and a pay button to confirm their selection.
- **Expected time of arrival**: Once the order is placed, the user is navigated to a screen that displays the estimated delivery time for the ordered item. The screen has real-time updates and shows the current status of the delivery and estimated arrival time with a progress bar.

#### Operator screens
- **Operator map**: This is the equivalent of the user map for the operator. It includes all the features of the original map, as well as displaying all orders in the area as pins on the map, color-coded to their status.
- **Pending orders screen**: This is a more detailed view of the pending orders. It displays information on items ordered, user location, and time of order. Also, it gives operators the ability to sort and search orders. The interface is a clear listing format with easy access to detailed order information.
- **Order accepted screen**: Once an operator accepts an order they navigate back to the map but with just their location and the pin of the accepted order.


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


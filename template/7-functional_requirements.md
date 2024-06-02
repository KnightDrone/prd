# Functional Requirements

## Key Features of the MVP

### Location-Based Ordering

Users have the capability to place orders for essential supplies directly from their current location through an intuitive map interface. This system significantly enhances convenience and accessibility, even in the most remote areas. The primary functions include an interactive map interface, real-time location tracking, and the ability to place orders directly from the map. These features depend on the phone’s location sensors, ensuring precision and efficiency.

Imagine being on a secluded camping trip and realizing you need additional supplies. With this system, you can effortlessly order what you need with just a few taps on your phone. The interactive map interface makes it easy to navigate and select your delivery location. Real-time location tracking ensures that your supplies are delivered accurately to your current position, eliminating the stress and uncertainty often associated with deliveries in remote locations.

### Order Status Updates

Users receive timely updates on the status of their orders, offering transparency and reassurance throughout the delivery process. The key functions include real-time notifications, order status tracking, and historical order tracking. Operators are notified when users place orders. This allow to reduce the time where we need to match an order to an operator.

### AI Chat Assistant
Users can engage in seamless communication with an AI chatbot for any outdoor-related queries, enabling them to swiftly access valuable information. This functionality is particularly beneficial for those seeking quick answers in dynamic environments, enhancing their overall experience and satisfaction.

The key functions encompass AI chatbot integration, which allows for an intuitive and interactive dialogue between users and the system. The chatbot excels in query processing and response generation, ensuring that users receive accurate and pertinent information promptly. For instance, a user planning a hiking trip might ask, “What are the weather conditions in Zermatt this weekend?” and receive detailed, real-time weather forecasts and recommendations for suitable gear.

Additionally, the system includes caching of previous conversation, allowing users to revisit and reference past interactions. This feature not only enhances convenience but also fosters a sense of continuity and reliability. A user can effortlessly access prior advice on preferred hiking trails or safety tips, providing a consistent and supportive resource.

### Operator Management Tools

Operators have access to intuitive management tools, including a specialized map interface highlighting pending orders and a dedicated screen for efficient order management. These tools are designed to streamline the order management process, making it easier for operators to handle and fulfill orders effectively.

The key functions include an operator dashboard, which provides a comprehensive overview of all operations, and a pending orders map interface that visually displays all orders awaiting action. This interface allows operators to quickly identify and prioritize tasks based on geographic location. Additionally, the system includes order acceptance and rejection functionality, enabling operators to manage their workload and ensure timely delivery of services.

For example, an operator can easily view a pending order on the map interface, assess its location relative to other orders, and decide whether to accept or reject it based on current capacity. This capability not only enhances operational efficiency but also contributes to higher customer satisfaction by ensuring that orders are managed and fulfilled in a timely manner.

### Offline Functionality

The map functionality operates seamlessly offline by downloading them, ensuring uninterrupted access to essential features in areas with poor connectivity. This ensures that users remain informed and capable of accessing vital information even without an active internet connection.

The key functions include offline map access, which allows users to navigate and utilize the map without needing connectivity. Caching of key data for offline use ensures that essential information, such as previously viewed locations or routes, is available when needed. Additionally, offline guides provide valuable resources and information about various outdoor activities, locations, and safety tips.

For instance, users can interact with the AI chatbot to ask questions and obtain information before embarking on a hike. Once they are in an area with limited or no connectivity, they can still access their previous conversations with the chatbot, ensuring they have the necessary guidance and information readily available. This offline functionality greatly enhances the reliability and usability of the map interface, providing users with confidence and security in remote or low-connectivity areas.


## Architectural Diagrams

### High-Level Architecture

Components:

- Client Application: Mobile app for users and operators (React Native)
- Backend Services: Firebase for database and authentication, Stripe for payment processing, OpenAI for AI chatbot functionality
- Drone Management System: Interface for operators to manage drone deliveries

## Key Internal Functionality

### 1. Location-Based Ordering
- **GPS Integration**: The mobile app integrates with the device's GPS to obtain the user's current location.
- **Map Interface**: An interactive map interface allows users to place orders based on their location.
- **Order Processing**: Orders are sent to Firebase for storage and processing once placed.

### 2. Order Status Updates
- **Real-Time Notifications**: Users receive push notifications at key points in the delivery process, such as order confirmation, drone deployment, and delivery completion.
- **Status Tracking**: Users can check the status of their orders in the app at any time.

### 3. AI Chat Assistant
- **Query Handling**: Users can ask questions via the chat interface, which are processed by the OpenAI backend.
- **Response Generation**: The AI generates appropriate responses based on context and provides relevant information to the user.

### 4. Operator Management Tools
- **Order Management**: Operators can accept or reject orders and manage the delivery process. Operators have access to screens that provide an overview of pending, ongoing, and completed deliveries.

### 5. Offline Functionality
- **Data Caching**: Key data, including maps and order details, are cached on the device for offline use.

By adhering to these functional requirements, Wild Knight will ensure a robust and reliable MVP that addresses the needs of both hikers and operators, providing a seamless and innovative solution for outdoor enthusiasts.

# User Analytics and Acceptance
### Analysis plan
To gather user analytics we will use the firebase google analytics library. This will allow us to track certain user events and define our own custom events to allow us to better understand how our app is being used. With the addition of firebase's Crashalytics, we will have the full picture of the usage and performance of the app, allowing us to make informed decisions on development and bug-fixing.

### Key metrics
- **Active users**: How frequently users log on to the app and how long they stay.
- **Churn rate**: How many users drop the app within a given period of time.
- **Session length**: Time spent on app overall and each screen individually.
- **Order fulfillment time**: How average delivery time compares to expected time calculated.
- **Delivery success rate**: What percentage of deliveries arrive at user without issues or returns.
- **User retention**: How many users return to the app after their first use.

### Success criteria
- Low churn rate: we would like to keep it below 50%.
- Appropriate session length: it is desirable to have users engage with our app, however keeping users on the app for a long time is not our goal. The order process should be seamless and quick, we will monitor how long is spent on each screen to see if too much time is spent anywhere, this could be an indication of unintuitive UX.
- Low order fulfillment time: we would prefer the order fulfillment time is slightly lower than the expected time, but not by a large margin. This will maximise user satisfaction without making the expected time useless.
- High delivery success rate: it will be important to give a communication channel to allow users to communicate any issues with delivery. Since we are relying on operators for now, quality control will be challenging.
- High user retention: a high user retention rate will indicate that users find value in the app and are motivated to return after their initial use.

### User analytics
- Implement Google Analytics through Firebase for behavioral tracking.
- Implement Firebase Crashlytics for monitoring app stability.
- Anonymize data to comply with privacy standards.
- Monitor user engagement, feature use, conversion rates, user retention, and drop-off rates.
### A/B testing
- Test different navigation trees to find the most user-friendly layout/flow.
- Experiment with different formats of displaying order menus and delivery tracking.
- Try out different UX designs for given components to see which is most intuitive and maximizes user retention.
- Test different methods of communication between users and operators to see which is most effective.
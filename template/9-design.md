# Design and Implementation
## Frontend
Key Libraries and Languages:

- React Native with Expo framework
- TypeScript for type safety and better developer experience
- React Navigation for navigation stacks and tabs

Components Used:

Custom components for buttons, list items, bottom bars, search bars, cards, etc., stored in the components folder.
Navigation stacks and tabs defined in the navigation folder.

Essential Screens:

- Onboarding: These are the screens that facilitate onboarding of a user and filling in essential user information.
- Explore: This screen likely serves as the main hub for users to discover events, connect with others, and explore various features of the app.
- Profile: The Profile screen allows users to view and edit their personal information, including interests, academic pursuits, and profile picture. It's essential for customization and personalization within the app.
Maps: The Maps screen provides users with a visual representation of event locations, enhancing the event discovery and navigation experience.

## Backend
Functional Blocks:

- Firebase Authentication: Handles user authentication using Google Auth.
- Firestore Database: Stores user profiles, social network data, and messaging.

## Data Model

Announcements:
The Announcements model stores information about announcements, including titles, content, publication dates, and authors.

Events:
The Events model manages data related to events, including event titles, descriptions, dates, locations, and attendee lists.

Interests:
The Interests model stores user interests for personalized recommendations and matchmaking.

Users:
The Users model manages user profiles, including usernames, email addresses, profile pictures, and associated interests.

Notifications:
The Notifications model stores notification data, including sender, receiver, content, and timestamp, for communication between users.

Messages:
The Messages model manages message data between users, including sender, receiver, content, and timestamp for communication within the app.

### Organization and Storage

User data is organized into profiles and stored in Firestore Database.

Social network data is structured as a graph and stored in Firestore Database.

Event data is stored in Firestore Database with separate nodes for event details and attendee lists.

### Data Sharing/Copying/Caching

User data is shared and accessed by various components within the frontend application.
Social network data is retrieved and visualized dynamically based on user interactions.
Event data is cached locally on the device for offline access and updated periodically from Firestore Database.

## Security Considerations
Google Auth integration ensures secure user authentication.

Firebase Authentication and Database security rules are configured to restrict access to authorized users only.

Data encryption is applied to sensitive user information stored in Firestore Database and Firebase Authentication.

## Infrastructure and Deployment

Application development, testing, and deployment are managed using Expo Application Services (EAS).

CI/CD workflows are set up to automatically build and deploy APKs from the main branch using Expo CLI and EAS.

Firebase provides the backend infrastructure for user authentication, database.

## Test Plan
Unit testing is performed using Jest framework for frontend components and functionalities.

End-to-end testing is conducted using Maestro framework for testing app flows and interactions.

SonarCloud performs code analysis and identifies issues for resolution before merging into the main branch.

Special infrastructure requirements include integration with SonarCloud for code analysis and with Maestro for end-to-end testing.
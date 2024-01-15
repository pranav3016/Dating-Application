# Dating App Database

## Objectives

The goal of this project is to design a robust relational database for a dating app with the following features:

- Users can efficiently login/signup.
- Users can add details such as city, state, phone number, photos, etc.
- Users can express interest (like) in other users based on gender and relationship type preferences.
- Users can rate and block other users they have matched with.
- Users can engage in chat if there is a mutual match.
- Users have the option to choose between free and premium memberships.

## Business Problem

The dating app industry faces challenges that impact user experience and data integrity. Key issues include:

- Inactive user profiles reduce daily matches, impacting customer satisfaction.
- Users with inappropriate behavior need to be identified and addressed.
- Unverified users and multiple accounts for a single user contribute to data inconsistency.

## Solution Strategy

Our proposed solutions address these challenges through the following strategies:

- **Database Design Concepts:** Utilizing foreign key references with the ON DELETE CASCADE property to maintain data consistency and remove all associated records when a user is deleted.

- **Blocking Mechanism:** Introducing a block table to track user blocks. Implementing a threshold to identify highly blocked users and filter them from the platform.

- **Data Integrity Measures:** Enforcing UNIQUE and NOT NULL constraints to prevent users from signing up with the same phone number and passport number, ensuring genuine user profiles.

- **Efficient Data Retrieval:** Optimizing data retrieval by dividing user information into smaller tables with various primary key-foreign key relationships.

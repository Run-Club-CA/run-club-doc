# T3A2 - Part A

## Run Club MERN full stack application

### Authors: Laurence Walton and Liam Massey

***

### Table of Contents

- [Purpose](https://github.com/Run-Club-CA/run-club-doc#purpose)
- Functionality/Features
- Target Audience
- Tech Stack
- Dataflow Diagrams
- Application Architecture Diagram
- User Stories
- Wireframes
- Project management screenshots

***

### Purpose

A New South Wales running and sports shoe store has a local running club located in Waverley, that has for the most part been organized by using facebook.  
The owners of the store feel that although their group on facebook has been useful, its also created some challenges such as updating and cancelling events due to unforeseen circumstances, having a more easier to understand calender, and not being as user friendly as they would like.  

The purpose of the Run club application is to address these issues and create a user friendly, community driven and welcoming place. The application will allow regular users to view upcoming events, keep track of any changes to events and track their own progress with how many kms have been run from completed events. Where the app will also benefit the trainers by giving them better autonomy with scheduling their events, as well as being able to update or cancel events with ease and check off completed runs for attendees.  

The running club is looking to create an app that promotes a healthier lifestyle, is community focused and inclusive.

***

### Functionality/Features

- **User Creation**: Main feature allows users of the application to create their profile. This includes adding their name, age, email, and password to an account. Users can also update their details on the profile and delete their account if required.
The features of updating and removing an account require the user to be logged in, which will
have the use of JWT authentication.  
- **User Login/Logout**: The user is required to login to the application to view upcoming events/sign up for events etc. Sign up will require the users email and password. Upon authentication the user will be assigned a JSON Web Token that will help reduce the amount of times a user will need to sign in. Users can log out as well when logged in.
- **Admin extras**: As an admin user type, there are permissions that are allowed such as making a regular user a trainer and removing that status.
Admins can also see a list of all users in the app and search for a user using their name.
- **Homepage/dashboard**: Upon signing up the user will be able to view their profile, along with information of upcoming events they are signed up too. Profile will include amount of KMs ran so far for the user.
- **Event Creation**: Trainers and Admin users are able to create an event and post it up on the calender/event page. This will require information such as the Location, Time, Distance and Difficulty.
- **Event Update/Delete**: Trainers and Admin will be able to remove and update event details of created events. Admin will be able to have access to all events, where trainers only have access to their events for updating and deleting.
- **Event page/calender**: A page will be created that can be navigated too by the user, this event page will have a calender that details what events are coming up and their difficulty. From here Users will be able to sign up to attend.
- **Event Attendance**: Any user is allowed to sign up to attend an event. They are also able to remove themselves from attendance.
- **Completed Run**: Trainers are able to check off the participants of an event after it has happened. This allows the kms to be tracked for users, which adds to the total kms run by that user.

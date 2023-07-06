# T3A2 - Part A

## Run Club MERN full stack application

### Authors: Laurence Walton and Liam Massey

***

### Table of Contents

- [Purpose](https://github.com/Run-Club-CA/run-club-doc#purpose)
- [Functionality/Features](https://github.com/Run-Club-CA/run-club-doc#functionalityfeatures)
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

***

### Target Audience

The core users of the app would be individual runners of all fitness levels from fairly new runners to the highly experienced. These users want to be easily connected with like-minded individuals for social engagement, motivation, and to run with trainers to become more skilled about running. The app users would mostly fall between 15-55, cover all genders, income levels, education levels, and marital/parenthood statuses. Geographically, users would live within the Sydney metropolitan area most likely within 20 kilometres of the store location, Waverley. Psychographically, they are likely to be strongly interested in health/fitness, highly social, open to new experiences, and somewhat competitive.

Secondary users would be the run leaders/trainers, who are highly experienced runners who may be volunteers or employees of the running shoe store. They are social, enjoy sharing their passion for running through group runs, and find satisfaction through improving other runners of all levels with their coaching abilities and knowledge of running techniques/gear.

***

### Tech Stack

**Front-end:** HTML5, CSS3, JavaScript, React, TailwindCSS

**Back-end:** Node.js, Express

**Database:** MongoDB

**Testing:** Jest

**Design:** Figma

**Deployment:** Heroku, Netlify

**Project management/Communication:** Trello, Notion

*** 

### User Persona: Runner

Tom is a 28-year-old male who works on the marketing team of a local brewery. He is a beginner-to-intermediate level runner trying to lead a healthier lifestyle. Joining a local running group was an easy choice for Tom who thought it would help him to stay accountable with his running schedule while meeting friendly locals who shared in his running interest.

Tom has found it to be frustrating to coordinate his schedule with the club's events due to work commitments and the current clubs lack of a proper schedule/calendar. He currently tries to loosely track his kilometres run based on the estimated length of the runs he joins, but would appreciate a more structured run tracker which could also track his progress against other run club users and give him some some extra motivation to show up and push his running further.

#### **User Story: Runner**

- As a runner, Tom would like to signup/login to the app so his experience can be personalised and secure.
- As a runner, Tom would like to find upcoming runs so that he can see which runs fit his schedule.
- As a runner, Tom would like to see the length and difficulty of runs so that he can join runs which match his running abilities.
- As a runner, Tom would like to sign up for runs so as to see the runs he will be attending.
- As a runner, Tom would like to have the runs he completes tracked so that he can track his performance, be rewarded for his consistency, and compete with his friends.
- As a runner, Tom would like to cancel runs he has signed up for but can no longer attend so that they won't show up in his run list and to help the coaches anticipate numbers better.
- As a runner, Tom would like to be notified if a run he has signed up for is being cancelled due to weather etc so that his time isn't wasted traveling to the run and he can schedule other activities at that time.
- As a runner, Tom would like to know how many runs/how many kms he has run in the last week/month so that he can track my metrics for motivation and track his progress towards fitness goals.
- As a runner, Tom would like to compare his stats with other runners to gamify his experience, compete with friends, and be rewarded for hitting milestones.
- As a runner, Tom would like to see the forecasted weather on his runs so he can wear appropriate gear.
- As a runner, Tom would like to access a playlist so he can have curated and encouraging music which also results in a shared listening experience with other members.

### User Persona: Trainer

Alicia is a 32 year old trainer that volunteers for the run club. When she isn't hosting running events she is working as an air traffic controller, or living a busy social life. Alicia is an outgoing person that loves to be challenged and help others achieve and beat their goals.  

Alicia finds that the running group she volunteers at is a great way to be engaged within the community, but has found issues with the way its organised. Due to her busy schedule, trying to organise events around other trainers can be difficult without a proper calender. She would love to see the running group be able to have a much more centralized and easy to use app to co-ordinate runs.  

#### **User Story: Trainer**


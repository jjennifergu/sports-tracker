# score!

## score!: The Big Red ESPN

An app designed for all Cornell sports enthusiasts, score! helps its users keep track of Cornell sporting events. The purpose of score! is to make tracking and keeping up with Cornell sports easier for Cornell's incredibly busy students. It is an app which, on its backend, maintains an API of Cornell sporting events, Cornell teams, and users. A team can host many events, and each event is owned by exactly one Cornell team. The backend provides an API which holds all the events that teams have posted, serialized into accessible and readable data about the event for the frontend. On the frontend, data is retrieved from the provided API and organized so users can filter, sort, and view both completed and upcoming Cornell sporting events. Users are able to filter upcoming events by both the gender and sport (i.e. Men's Soccer, Women's Tennis). Users are also able to access a complete list of a specific team's record. When viewing an event, users see its time, date, and location (and if the event has been completed, the outcome of the game). 

## Feature Highlights
<img height="700" alt="ss1" src="https://user-images.githubusercontent.com/82056699/144698115-671e0685-0843-4fe3-8849-38aedd04fa91.png"> <img height="700" alt="ss2" src="https://user-images.githubusercontent.com/82056699/144698093-1b4e7336-fac8-4921-a512-03071f4d1b7d.png"> 

Upon launching, the home screen is loaded, where the next upcoming sports event is displayed at the top, along with the team, opponent, date, time, and location. More upcoming events are displayed below in a horizontally-scrollable collection view, including the date, team, opponent, and location. The “see all” button can be clicked to open the upcoming events page.  

<img height="700" alt="upcoming1" src="https://user-images.githubusercontent.com/57200368/144732037-89644aea-f176-4765-948d-96434d001174.png"> <img height="700" alt="upcoming2" src="https://user-images.githubusercontent.com/57200368/144732045-c5436c56-c8e4-4799-b881-c7a0dd7a002f.png">

On this page, all upcoming events can be viewed and searched through using gender and sport filters. The team, location, time, date, and opponent is displayed for each upcoming event.

<img height="700" alt="sport1" src="https://user-images.githubusercontent.com/57200368/144732053-2396a25f-bcb9-44e3-bb48-b31196db69f6.png"> <img height="700" alt="sport2" src="https://user-images.githubusercontent.com/57200368/144732054-6c79333f-cd4f-479a-a3f0-d74c5cf3a208.png">

Sporting events can also be browsed by team. By clicking on a team on the home page, a new page is pushed with the complete record of the team's past and future games. The date, opponent, and location is displayed for each of these events. If the event has already occurred, the result is displayed as well.

## iOS
- Utilizes NSLayoutConstraint
- Implements UICollectionView
- Uses UINavigationController to navigate between screens
- Integrates the API provided by backend members for data retrieval of the event information
   
## Backend
Repo: https://github.com/DylanMcCreesh/AppdevHackChallenge
- API implements 14 routes (including GET, POST, and DELETE methods)
- Database houses three tables (Fan, Team, and Event Tables) and an association table between the Fan and Team tables, as well as relational keys between the Event and Team tables
- API specification is provided for all 14 of the routes on backend repo

## Next Steps
Some routes are not currently utilized on the frontend. We believe in the future these routes could be implemented to enhance the features and functionality of the app. For example, routes for users to create password-protected accounts and to select favorite teams can be implemented on the frontend in the future.

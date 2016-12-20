+++
date = "2016-12-20T16:44:08+11:00"
title = "Event Manager Android Application"
draft = false

+++

**(August 2014 - October 2014)**  
**Solo Project**

An Android application which manages events. Users can add events and their details into the app, such as
time, title, location and any notes. The app will estimate the travel time between the current location
and the event's location using Google Distance Matrix API. Using the estimated travel time, the app will
alert the user when it's the best time to leave for the next event.

### Functionality and features

*   Users can add events, as well as edit and delete existing events.
*   The app will alert users when it's the perfect time to travel to the next event, using GPS and Google Distance Matrix API.
*   When adding new events, the app will check if the new event can fit into the current schedule (also takes into account travel times).
*   Modular design with Hierarchical MVC architecture.
*   Has two views (calendar view and list view) on different fragments.
*   Uses persistent storage with SQLite.
*   Queries the Google API when there's Internet connectivity and uses GPS if its available.
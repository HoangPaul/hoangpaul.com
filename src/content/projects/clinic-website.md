+++
title = "2014 Web Database Applications"
date = "2014-11-10T12:43:19+11:00"
draft = false

+++

A student project for Web Database Applications, Semester 2 2014.
## Clinic
#### At a glance
A website where people can create bookings with doctors. Doctors specify their timeslots, patients can book their own appointments.
#### Current functionality
**Doctors** can specify their available timeslots, as well as view information about patients who has made a booking with them (and only their patients information) and contact information.
**Patients** can browse from a list of doctors and view their location using Google Maps. They can choose a doctor and make a booking, which then no one else can book unless the patient cancels.
#### Advanced features:

##### Security
* Isolated database and webserver behind an Amazon firewall to protect against unauthorised access.
* Database is encrypted, key is stored separately on a different server, encryption/decryption is done on database server.
* HTTPS everywhere.
* Utilised security features provided by the CakePHP framework.

##### Google Maps API
* Each doctor belongs to a clinic. You can see the location of that clinic with Google Maps.

##### Authentication/Session
* Both doctor and patient session management using CakePHP. Some features are only accessible to certain users. Doctors, for instance, can can view other patients records.
* Server-side and client-side validation.

##### Large database
* Particularly large database with god know’s what’s happening.
* Basic search

##### Documentation
* PDO helpers are documented using PHPDocumentor.

#### Roles and contributions:
* **Trung Dai**
(Team Leader, PHP, convert HTML to CakePHP+HTML)
* **Paul Hoang**
(PHP, security, convert HTML to CakePHP+HTML, presenter)
* **Cong Anh Duy Trinh**
(Database schema, database data generation)
* **Luke Clifopoulos**
(Database schema, database data generation)
* **Anh Bao Nguyen**
(Project leader + idea, functionality planner, HTML + CSS)
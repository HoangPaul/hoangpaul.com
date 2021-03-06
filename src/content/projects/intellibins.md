+++
title = "IntelliBins (Spotless Hack @ the G 2016)"
date = "2016-12-18T20:02:07+11:00"
draft = false
image = "intellibins/intellibins-webapp.jpg"
flavorText = "Who would have thought bins could be so interesting?"

[[images]]
url = "intellibins/intellibins-webapp.jpg"
caption = "IntelliBins web view"

[[images]]
url = "intellibins/intellibins-webapp-android.png"
caption = "IntelliBins web view and native Android application"

[[images]]
url = "intellibins/intellibins-hardware.jpg"
caption = "IntelliBins sensor prototype"

[[images]]
url = "intellibins/intellibins-bin.jpg"
caption = "IntelliBins sensor for live demo"

+++

Team: David Lei, Erfan Norozi, Kenny Yu, Patrick Shaw, Paul Hoang, Ramzi Hossari

We created a solution to track bin capacity and allow cleaners to proactively clean
bins before they spill over. Our solution was created and presented at
[Spotless Hack @ the G](https://spotless-hack-the-g.devpost.com/) and was awarded a
position as a [finalist](https://devpost.com/software/intellibins).

Three teams (including ourselves) had independently come up with this idea, but we
like to think we were first.

Special shoutout to Patrick for being a great mentor!

#### Project details

We have created an IoT device that uses ultrasonic waves to determine a bin's capacity and
transmits this information to a centralised server for data analysis and visualisation.

Using an Android application, cleaners have real-time information to identify
bins nearing capacity so that they can attend to them before they overflow.

Managers can identify problem areas through visualisation tools via a web application.
This information can also help plan for future infrastructure projects.

* [View website <i class="fa fa-external-link" aria-hidden="true"></i>](https://hoangpaul.github.io/intellibins/)
* [View web demo <i class="fa fa-external-link" aria-hidden="true"></i>](https://hoangpaul.github.io/intellibins/web-demo/)
* [<i class="fa fa-github" aria-hidden="true"></i> View website source](https://github.com/HoangPaul/intellibins)
* [<i class="fa fa-github"aria-hidden="true"></i> View web demo source](https://github.com/HoangPaul/spotless_web_frontend)

### Technologies used

#### Frontend website
* React
* Material Design
* Google Maps JavaScript API

#### Backend
* Node.js
* Express
* SQLite

#### Android Application
* Java

#### Physical sensor
* Arduino
* Raspberry Pi
* Distance sensor using ultrasonic waves
* Python

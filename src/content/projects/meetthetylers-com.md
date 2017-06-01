+++
title = "meetthetylers.com"
date = "2016-08-08T20:13:54+11:00"
draft = false
image = "meetthetylers/meetthetylers.com.jpg"

[[images]]
url = "meetthetylers/meetthetylers.com.jpg"
caption = "Website screenshot"

[[images]]
url = "meetthetylers/meetthetylers-responsive.png"
caption = "Responsive design"

+++

A [static site for my sister's wedding](https://www.wedding.meetthetylers.com).

## Static Site Generator

As part of this project, I had written a static site generator in Node.js
to make content changes easier. The static site generator had the following features:

* Web-based WYSIWYG editor with image manipulation.
* Ability to preview the changes before deployment.
* Ability to deploy to live with one click.
* Ability to specify RSVP form target email address.

[<i class="fa fa-github"></i> Static site generator source](https://github.com/HoangPaul/wysiwyg-meetthetylers.com)

### Technologies used

#### For the static site generator
* Node.js
* Express

#### For the generated site
* Bootstrap
* jQuery
* AWS (EC2, S3, CloudFront)
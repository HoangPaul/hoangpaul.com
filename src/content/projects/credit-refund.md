+++
title = "Credit Refund"
date = "2016-01-02T20:13:39+11:00"
dateEnd = "2016-11-01T20:13:39+11:00"
draft = false
image = "creditrefund/creditrefund.com.au.png"
flavorText = "My first (very) small business"

[[images]]
url = "creditrefund/creditrefund.com.au.png"
caption = "Credit Refund website"

[[images]]
url = "creditrefund/creditrefund-android.png"
caption = "Credit Refund Android application"

+++

An [Android app](https://creditrefund.com.au/) with a Node.js backend that allows users to exchange their
spare Google Play Credit into cash.

This was also my first foray in managing a small business. This project taught me a lot about
starting a business from scratch, the endless amounts of paperwork, funky tax obligations
and the pain of getting people to use your product.

The reason I took it off the Play Store was the potential fraud risk. There was a person who made
a purchase and quickly refunded it. Normally, I would have lost the $5, but I was luckily protected
by an obscure software bug and the $5 was never sent.

[<i class="fa fa-github"aria-hidden="true"></i> Node.js backend source](https://github.com/HoangPaul/creditrefund-api)  
[<i class="fa fa-github"aria-hidden="true"></i> Static site source](https://github.com/HoangPaul/creditrefund-static)

### Technologies used

* Node.js
* Express
* mocha
* nginx
* Docker
* Java (for the Android application)
* AWS (EC2)

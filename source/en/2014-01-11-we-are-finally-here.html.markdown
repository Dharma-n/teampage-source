---
title: We are finally here
date: 2014-01-11 00:04 UTC
tags:
---

####Intro
After almost a month, our team finally get to release our first version of [Senkyoyarou.com](http://senkyoyarou.com), of which the meaning in Japanese Language is __"Let's go voting"__. Me and Mr. N both has more than 5 years of web developing experience, with multipule languages and frameworks like __Django__, __Rails__, etc. And this time we wanted something different.

####What
The website, [Senkyoyarou.com](http://senkyoyarou.com) aims to expand the awareness of Japanese people ( Or people of anyother democracy country ) on voting, by showing support rate of particular senator or political issue __real time__, making it more efficient for people to catch the current situation.

####The system
To handle the heavy traffic and the need of realtime websocket processing, we found the currently popular nodejs handy to our needs, with a few obvious flaws:

*	Readability of Javascript Code is just horriable
*	Callback Hell
*	Memory Leaking issue sometimes happen		

and it's obvious merits:

*	Javascript on both ends makes it faster to develop
*	Rich resource to explore on npm
*	Native support of websocket
*	Native Async processing of request
*	Easy to port to mobile with the same code base

####Dharma

Dharma is what we made, with [backbone.js](http://backbonejs.org) and [underscore.js](http://underscorejs.org) to handle [stateless](http://en.wikipedia.org/wiki/Stateless_protocol) front-end, with user login, click events, modules and so on. It will ease people's way of creating [stateless](http://en.wikipedia.org/wiki/Stateless_protocol) websites. It is also very light, so that it'll also be handy while creating __mobile applications__.
---
layout: page
title: Invenio Mobile
description: >
    A hybrid mobile app for the Invenio document repository, written during my summer at CERN.
category: project
permalink: /projects/invenio-mobile/
sitemap:
    lastmod: 2015-09-11
---

<figure>
	<div class="pure-g">
		<div class="pure-u-1-3"><img alt="Screenshot of the app's search screen on Android" src="{{site.baseurl}}/img/projects/invenio-mobile/android/search.png"></div>
		<div class="pure-u-1-3"><img alt="Screenshot of the app's results screen on Android" src="{{site.baseurl}}/img/projects/invenio-mobile/android/results.png"></div>
		<div class="pure-u-1-3"><img alt="Screenshot of the app's record screen on Android" src="{{site.baseurl}}/img/projects/invenio-mobile/android/record.png"></div>
	</div>
	<figcaption>Screenshots of the Invenio Mobile app on Android.</figcaption>
</figure>

In the summer of 2014, I took part in the [CERN openlab Summer Student programme][openlab-ss], for which I worked on a mobile app for the [Invenio document repository][invenio], the open-source system behind the CERN Document Server. I gave [a lightning talk][lightning-talk] about it, which won third prize on the programme!

Invenio is a Web service written in [Python][] and [Flask][], which allows users to publish, browse and download papers or other documents. A prototype had been created for a mobile app which would allow users to browse Invenio repositories. My objectives were to improve its speed, functionality and usability, either by building on the prototype or starting over. I chose to start over, due to the large differences in architecture and chosen frameworks.

<figure>
	<div class="pure-g">
		<div class="pure-u-1-3"><img alt="Screenshot of the app's search screen on iOS" src="{{site.baseurl}}/img/projects/invenio-mobile/ios/search.png"></div>
		<div class="pure-u-1-3"><img alt="Screenshot of the app's results screen on iOS" src="{{site.baseurl}}/img/projects/invenio-mobile/ios/results.png"></div>
		<div class="pure-u-1-3"><img alt="Screenshot of the app's record screen on iOS" src="{{site.baseurl}}/img/projects/invenio-mobile/ios/record.png"></div>
	</div>
	<figcaption>Screenshots of the Invenio Mobile app on iOS. These screens are defined by the exact same HTML as those in the Android screenshots above.</figcaption>
</figure>

The app was built using [Apache Cordova][], a hybrid app framework which allows HTML5 apps to be wrapped and deployed to Android, iOS and many other platforms. This is very useful for building simple cross-platform apps, but raises interesting security issues, as Cordova apps are vulnerable to Cross-Site Scripting. The Invenio app was to display content differently depending on which server it was connected to, meaning that I had to create a simple way to customise the display of records without using HTML (which could contain malicious scripts from a compromised server).

Within the Cordova framework, I used [jQuery][], [JinjaJS][] for templates, and [TaffyDB][] (a JavaScript database library for semi-structured data). I found the [Ratchet][] CSS framework particularly useful for making the app look native on both Android and iOS.

[openlab-ss]: http://openlab.web.cern.ch/summer-student-programme
[invenio]: http://invenio-software.org/
[lightning-talk]: https://cds.cern.ch/record/1750935?ln=en
[Python]: https://python.org/
[Flask]: http://flask.pocoo.org/
[Apache Cordova]: https://cordova.apache.org/
[jQuery]: https://jquery.com/
[JinjaJS]: https://github.com/sstur/jinja-js
[TaffyDB]: http://www.taffydb.com/
[Ratchet]: http://goratchet.com/

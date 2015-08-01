---
layout: page
title: GO Publisher Web UI
description: >
    A Web UI for job control I created during a summer internship at <a href="http://www.snowflakesoftware.com/">Snowflake Software</a>.
category: project
permalink: /projects/go-publisher-web-ui/
legal_gumph: >
    Screenshots &copy; 2015 <a href="http://www.snowflakesoftware.com/">Snowflake Software</a>, all rights reserved.
---

<figure>
	<img alt="Screenshot of GO Publisher Workflow's overview screen" src="/img/projects/go-publisher-web-ui/overview-screen.png">
	<figcaption>GO Publisher Workflow's overview screen, showing all jobs currently in the system.</figcaption>
</figure>

In 2013, I won the [Snowflake Software Code Off](http://www.snowflakesoftware.com/2013/03/code-off-2013/) at the University of Southampton, and spent the summer working for Snowflake Software on a Web interface for their data publication platform, [GO Publisher Workflow][gpw].

As a system which runs large data processing jobs, GO Publisher Workflow needs a way for users to create jobs, monitor progress, and download the results. My interface presents jobs in a clear three-column view, with jobs moving from left to right as they progress through the system. The user can drop files onto the interface to start jobs, and drag jobs between columns to change their status (for example, to start a waiting job). Within a job, individual tasks can be managed, and error logs or validation reports displayed.

<figure>
	<img alt="Screenshot of GO Publisher Workflow's job screen" src="/img/projects/go-publisher-web-ui/job-screen.png">
	<figcaption>GO Publisher Workflow's job screen, showing a single job, with all the files it has produced. The design is unchanged from my original, except the sidebar, which was added after I finished.</figcaption>
</figure>

The interface is written in HTML5, using Less with Bootstrap for styling, and CoffeeScript with jQuery for functionality. I was responsible for the whole process, from requirements gathering and user interface design, to writing code and integrating the interface with the main product.

[gpw]: http://www.snowflakesoftware.com/products/gopublisher/workflow/


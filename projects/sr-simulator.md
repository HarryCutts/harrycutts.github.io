---
layout: page
title: Student Robotics Simulator
description: >
    A simple robot simulator written in Python.
category: project
permalink: /projects/sr-simulator/
---

<figure>
	<img alt="Screenshot of the simulator with four robots playing in a virtual arena." src="{{site.baseurl}}/img/projects/sr-simulator/screenshot.png">
	<figcaption>A screenshot of the simulator, with four robots (in blue) pursuing a number of wheeled tokens (orange). The gray boxes represent barriers.</figcaption>
</figure>

During my time at Southampton University, and as part of my volunteer work with [Student Robotics][], I helped to run three [Smallpeice Computing and Microelectronics Summer Schools][summer-schools]. I took responsibility for running the programming workshops, for which I wrote a basic simulator to allow the participants to try out their ideas. It is now used for this summer school every year, as well as the main Student Robotics competition.

[The simulator][srobo-page] provides [an API][srobo-page-api] through which the user can control a virtual robot, which is designed to be as similar as possible to the API for the real Student Robotics kit. The user writes their program in Python and can then run it in a simulated arena, which contains the same obstacles, markers, and objectives as the arena in which they will compete. A game with up to four virtual robots can be simulated.

The simulator uses [PyGame][] and the [PyPyBox2D][] physics engine, allowing it to be run using a [Portable Python][] installation without administrator rights on Windows. ([ZIP files for Windows, Linux and Mac OS X][srobo-page] are available from the Student Robotics website.) The source code is available [on GitHub][github-project].

[Student Robotics]: https://www.studentrobotics.org/
[summer-schools]: http://www.smallpeicetrust.org.uk/residential-courses/computing-and-microelectronics/
[srobo-page]: https://www.studentrobotics.org/docs/programming/simulator
[srobo-page-api]: https://www.studentrobotics.org/docs/programming/simulator#Interface
[PyGame]: http://pygame.org/
[PyPyBox2D]: https://github.com/pybox2d/pypybox2d
[Portable Python]: http://portablepython.com/
[github-project]: https://github.com/HarryCutts/sr-turtle

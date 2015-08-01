---
layout: page
title: Student Robotics Control Interface
description: >
    An interface to allow <a href="https://wwww.studentrobotics.org/">Student Robotics</a> competitors to manually test their robots' hardware.
category: project
permalink: /projects/sr-mci/
---

<figure>
	<img alt="Screenshot of the interface's IO panel, with a diagram of a power board" src="{{site.baseurl}}/img/projects/sr-mci/io-panel-framed.svg">
	<figcaption>
		Screenshot of the IO panel, shown within a diagram of the power board. The left panel lists the connected boards, allowing one to be selected for control.
	</figcaption>
	<!-- TODO: PNG fallback -->
</figure>

As part of my volunteer work for [Student Robotics][], I created a user interface to allow our custom-designed kit to be controlled using our power board's built-in screen and buttons.

The power board (which has since been replaced) had a low-resolution 4.3in display, two buttons, and two depressible dials. The left dial was used to switch between panels, leaving only two buttons and the right dial for manipulating the selected panel itself. Combined with the restricted screen space and the need for intuitive design, this made designing the more complex panels quite challenging.

<figure>
	<div class="pure-g">
		<img class="pure-u-1-2" alt="Screenshot of the servo control panel" src="{{site.baseurl}}/img/projects/sr-mci/servo-panel.png">
		<img class="pure-u-1-2" alt="Screenshot of the motor control panel" src="{{site.baseurl}}/img/projects/sr-mci/motor-panel.png">
	</div>
	<figcaption>
		Screenshots of the servo (left) and motor (right) control panels.
	</figcaption>
</figure>

To allow the competitors to get started with the control interface quickly, context-sensitive help messages were provided throughout. Due to the restricted screen space these had to be very succinct.

In the two years in which it was used, the control interface proved very popular, and I received much positive feedback. Later, the power board was replaced with a new design, in which a separate tablet was used for control, and the interface was retired. The source code is still available [on GitHub][github-project].

[Student Robotics]: https://www.studentrobotics.org/
[PyGTK]: http://pygtk.org/
[github-project]: https://github.com/HarryCutts/sr-control

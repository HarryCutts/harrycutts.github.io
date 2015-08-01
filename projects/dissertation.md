---
layout: page
title: Autonomous Landing Site Selection (Dissertation)
description: >
    My dissertation project, on Autonomous Landing Site Selection for Micro Aerial Vehicles.
category: project
permalink: /projects/dissertation/
---

<figure>
	<img alt="Diagram showing a quadcopter flying back and forth over uneven terrain"
		src="/img/projects/dissertation-terrain.svg">
	<!-- TODO: PNG fallback -->
	<!-- TODO: test on IE (http://caniuse.com/#search=svg) -->
	<figcaption>
		A diagram of a method of scanning terrain using ultrasound, which I proposed
		before rejecting it due to low resolution of such a scan.
	</figcaption>
</figure>

My third-year project at the University of Southampton was on autonomous landing site selection for micro aerial vehicles (such as small quadcopters). As well as experimenting with ultrasound terrain scanning, I created a real-world partial implementation of the algorithm from Park and Kim's paper, ["Landing site searching algorithm of a quadrotor using depth map of stereo vision on unknown terrain,"][ParkKim2012] which uses data from a simulated 3D scanner to find suitable landing sites.

My implementation used an [ASUS Xtion PRO Live 3D scanner][xtion-pro-live] (similar to Microsoft's Kinect), which was originally going to be mounted on a [Parrot AR.Drone][ar-drone]. Unfortunately, due to weight and difficulty controlling the AR.Drone in suitable indoor spaces, I had to resort to fixing the 3D scanner in place and moving various items to create a 'landscape' below it. Within that landscape, my algorithm (an improved version of Park and Kim's) identified potential landing sites, highlighting them on a computer screen.

The system was written in Python, and used [Robot Operating System][ros] to connect to the 3D scanner (and originally the AR.Drone's controller and sensors).

Park and Kim's proposed algorithm is fairly simple; essentially, it finds the largest circle of smooth (though not necessarily horizontal) terrain in a depth map. After implementing as much of it as I could using a fixed 3D scanner, I made a couple of improvements, adding a method for assessing the slope of a potential site, and using aircraft dimensions to allow it to determine whether the aircraft could fit in much smaller sites than its bounding circle would suggest.

<figure>
	<iframe src="https://player.vimeo.com/video/95149059?title=0&byline=0&portrait=0" width="500" height="400" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen>
		<a href="https://vimeo.com/95149059">Third-year Project Viva Demo</a> from <a href="https://vimeo.com/harrycutts">Harry Cutts</a> on <a href="https://vimeo.com">Vimeo</a>.
	</iframe>
	<figcaption>
		<a href="https://vimeo.com/95149059">A video</a> that I showed during my viva, showing the system identifying landing sites in real-time with a fixed 3D scanner. The top-left window shows the depth map from the scanner, and the bottom-right shows the output of the algorithm. Circles indicate potential landing sites. Green circles are acceptable sites, orange circles are sites which are too small, and purple sites are too steep for a safe landing.
	</figcaption>
</figure>

[ParkKim2012]: http://arc.aiaa.org/doi/abs/10.2514/6.2012-2588
[xtion-pro-live]: https://www.asus.com/Multimedia/Xtion_PRO_LIVE/
[ar-drone]: http://ardrone2.parrot.com/
[ros]: http://www.ros.org/

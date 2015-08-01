---
layout: page
title: Clangers Demo
description: >
    My coursework demo for my computer graphics course, involving a Clanger and a badly-flown spacecraft.
category: project
permalink: /projects/clangers-demo/
legal_gumph: >
    The Clangers identity is copyright &copy; Peter Firmin and Oliver Postgate. I am in no way associated with or endorsed by the BBC, Smallfilms, Peter Firmin or Oliver Postgate. For texture and code credits, see <a href="https://github.com/HarryCutts/comp3004-coursework#credits">the README on GitHub</a>.
---

While at the University of Southampton, I took [a course in Computer Graphics][comp3004]. The coursework was to create a small 3D world based on [*The Clangers*](https://en.wikipedia.org/wiki/Clangers), a 1970s BBC children's program starring whistling rodents living on a small rock in space.

<figure>
	<iframe src="https://player.vimeo.com/video/83759625?title=0&byline=0&portrait=0" width="500" height="400" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen>
		<a href="https://vimeo.com/83759625">COMP3004 Coursework - The Clangers</a> from <a href="https://vimeo.com/harrycutts">Harry Cutts</a> on <a href="https://vimeo.com">Vimeo</a>.
	</iframe>
	<figcaption>
		<a href="https://vimeo.com/83759625">A video</a> of the action sequence built in to the demo.
	</figcaption>
	<!-- TODO: colour video controls according to site colour scheme (supported in Vimeo's embed options). -->
</figure>

I used [Blender][] to create the 3D models, which were then loaded into a C and OpenGL program as Wavefront OBJ files. The demo has a free-flying mode to let the user explore the scene, and a preset action sequence shown in the video above. [The source code](https://github.com/HarryCutts/comp3004-coursework) is available on GitHub.

[comp3004]: http://www.ecs.soton.ac.uk/module/COMP3004
[Blender]: https://www.blender.org/

## RQM Ecology topics

I've broken this into five chunks, assuming that we'll need to add a lesson on stats or just add more stuff. These are the big things I'd like to be able to cover.

Notes:
	- It might be best to combine lessons 1 and 2 in favour of more time spent on the analytic parts 

### Lesson 1. Qualitative review of population models

Main idea: 
	- modeling a population with a differential equation
	- gaining insight about a system in several ways without necessarily solving the equation

Topics:
	- phase portraits in 1 dimension - careful, it's not technically a phase portrait if one of the axes isn't a variable - draw the actual 1D phase portrait as well 
	- finding fixed points qualitatively
	- stability as the direction of a derivative - "stable", "unstable"
	- Examples: logistic equation and Allee effect

### Lesson 2. Qualitative population models in 2 dimensions

Main idea:
	- modeling interactions between multiple populations with a system of coupled differential equations
	
Topics:
	- introduce 2 dimensional phase portraits with both variables as axes
	- introduce null clines qualitatively
	- Examples: Lotka-Volterra predator-prey model and competition model

### Lesson 3. Fixed points, null clines, and stability 

Main idea:
	- can use math to find fixed points and null clines found by "luck" in previous lesson
	- can use math to find out if a fixed point is stable or unstable

Topics:
	- finding fixed points analytically
	- finding null clines analytically
	- stability analysis - this one is tricky and we might not get to it - probably better to do just graphically and computationally

### Lesson 4. Modeling in R

Main idea:
	- using R to plot, analyze, and solve population models

Topics:
	- calculating trajectories using forward finite difference 
	- plotting phase portraits in R
	- plotting null clines and fixed points - possibly solving in R as well?

### Lesson 5. Fitting models to data

This one I haven't thought out as much, but it could be what Martin suggested - fitting the Ricker model to some timeseries data.



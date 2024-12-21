# Laser Turret Project

This project involves using/developing a Raspberry Pi, the Command Terminal, a web interface, and Thonny (a python IDE) to craft a laser turret system. The robot system our team
decided on includes two stepper motors, 1 that controls azimuth and 1 that controls altitude. There is a laser connected to the output of the second motor to fire at targets 
relative to the origin (our initial position on the 5m x 10m grid). Our team of 3 scored 4/4 targets in phase 1, and 11/13 targets in phase 2, the highest in my class!

Here are outlines of the two phases that our robot had to perform as part of the final project:

Phase 1

The goal of phase 1 is to first read in its current location and all 13 target ids and corresponding coordinates (JSON file). Next, it is intended to sort the ids and coordinates
from 1 to 13 (using a dictionary) since the input target list was given out of order. Finally, our turret system fires at each target id sequentially, turning on the laser for 
3 seconds when pinned onto the target and turning off otherwise.

Phase 2

This is where things got well...tricky. The second phase involved targeting a shortlist of ids. For example, instead of all 13, we were given 4 target ids (not coordinates!) that we
would then pass through our online web interface to the turret system. The first step was to pass the 4 target ids via said interface. Next, the turret system truncated its original
list of 13 target ids into the given 4 with corresponding coordinates. Finally, it needed to optimize the path from its starting location and then follow through with the sequence. 
The optimization code initially found the best sequence of target ids and then go in that curated order.

I have attached a video of Phase 2 and a picture of our system to easily visualize it. It is hard to tell with the farther targets, but this run scored 4/4 targets. Enjoy!\

# ENME351 Final Project

My final project for ENME351 warranted me to use Sensing, Logic, and Actuation using Arduino to pass information over to Processing. I recreated the game Space Invaders with a few twists to meet my courses requirements. I included the following to demonstrate my understand of the key principles of the course: 

- A photoresistor to notify the user of their environment (light vs. dark)
- A button for the user to control light/dark mode in the Processing module
- A potentiometer to drag the turret left and right across the screen
- A second button to initiate a laser on the Processing module, and finally 
- A buzzer to play the intro to 7 Nation Army by The White Stripes once the game has concluded. 

The Processing module also displays a GIF (game over screen) to also indicate the end of the game. It was one of the features that made my project unique. Thank you for reading! Hope you enjoy the demonstration:

https://www.youtube.com/watch?v=vkBt0h3X4BA

# Assignment 1 RT2
----

creat a html documentation for the final assignment of RT1, a jupyter notebook for the same exercise and a confrontation of performance between the first assignment of RT1 and the code wrote by the professor

INSTALLATION
----
download in a ros workspace this package and press catkin_make

https://github.com/tommasodeangeli97/assignment1_rt2.git

to open the jupyter notebook 

$jupyter notebook --allow-root --ip 0.0.0.0

than open the folder assignment1_rt2 and inside open the notebook "assignment1_rt2.ipynb"

in order to start, use the two differnt terminals to launch

$roslaunch assignment1_rt2 simulation_gmapping.launch

$roslaunch assignment1_rt2 move_base.launch


# HTML DOCUMENTATION
----

You can find the documentation created using Sphinx here

https://tommasodeangeli97.github.io/assignment1_rt2/

Or directly from the repository settings->pages and clicking on the link appearing on the right

# CONFRONTATION BETWEEN THE FIRST ASSIGNMENT FROM RT1 AND THE CODE WRITTEN BY THE PROFESSOR
----
					
![image](https://user-images.githubusercontent.com/92479113/170602226-38b0f4d0-d2d0-4e9f-ad34-9679a4c65179.png)

So we can observe that the code written by the professor is, under all points of wiev, better than the code written by me

At this point i have taken in account the hypotesis Ha, the professor's code is faster than mine for the T-test; and for the Chi-Square test I have taken null hypotesis Ho, the two codes are indipendent one from the other
									
![image](https://user-images.githubusercontent.com/92479113/170603728-2feea46e-e6f5-42a4-8c01-34d2eb0f451e.png)


# JUPYTER NOTEBOOK
----

Using Jupyter Notebook I emplemented a user interface for the control of a virtual robot in a room reusing the code that I wrote for the last assignment of RT1 

# choosing the modality

to the user is given the possibility of choosing between 4 modalities: 0-mod are the instructions tu use the code; 1-mod is the automatic reaching of a point giving the 2D coordinates; 2-mod is a manual control for the robot; 3-mod is a manual control of the robot with an avoid collisions skill implemented

# modality zero

is a simple print of the instruction for using the user interface

# modality one

using differents widgets the user interface is completely interactable, enjoy following the instructions given on jupyter!

# modality two

using wigets type button is an implementation for substituting the teleop_twist_keyboard

# modality three

I reuse the same code wrote for the third modality of the precedent assignment adding the same structure of the second modality

# ATTENTION

the third modality and the second modality share some function (the VelocityCallback) and some global variables (linear, angular) so for using at best the two modality they has to be played both togeder

# plot of trajectory and laser scan

both of the plot are implemented in real time and they share the same class for plotting, as for the second and third modality is suggested to play those togeder, if the kernel result too busy there is the possibility of running the class and separately one plot or the other

# plot of the reached or not reached positions

this plot is created for having a visual proof of the accurancy for the first modality, the code will add on two fifferent global variable (rc, nrc) whenever the robot reach or doesn't reach the indicated point.
the plot is not in real time so has to be rerunned every time the user want to see that for aving the adjurned values
the globals variable are created in the first modality so for plotting this graf is mandatory running also the first modality

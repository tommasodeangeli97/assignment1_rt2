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

n.prove	p.temp(s)	m.temp(s)	p.crash	m.crash	p.wrong	m.wrong
1	162	0				8
2	165	389				2
3	168	422		1		4
4	0	0	1	1	2	2
5	165	0				2
6	0	0	1	1	1	7
7	164	0		1		1
8	167	0				6
9	166	390		1		1
10	167	395		1		4
Xi	1324	1596				
stand.dev	69,80162367	206,2383734				
pooled	23,26720789	68,74612447				
pooled^2	23703,26667					
p.std dev	68,85240252					
t stat	3,950479432					
deof	9					
i can conferm the null hypotesis with a 99.5 percent						
						
						
						
n.succ	8	4	2	6	2	10
n.fail	2	6	8	4	8	0
null hyp	6(10)		4(10)		6(10)	
deof	81					
x^2	3,333333333		3,333333333		3,333	
for the three the probaility of rejection the null hypotesis is between the 0.1 and the 0.05 that is not so significalnt, so i can't reject the null hypotesis						
![image](https://user-images.githubusercontent.com/92479113/170596484-59b66aa9-380e-470c-a73a-cde2fd8115ca.png)

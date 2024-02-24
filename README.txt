********************************* README ********************************************

Sarthak Swetang Shah (ssshah45@asu.edu)
CSE 579: Automated Warehouse

----------------------------------------------------------------------

The following is the implementation of the Automated Warehouse Scenario (ASP Challenge 2019)

- Files:

1) simpleInstances - Contains various initialization files (provided along with the project instructions) for checking the working of the system.
	- inst1.asp
	- inst2.asp
	- inst3.asp
	- inst4.asp
	- inst5.asp
    
2) convert_input.asp - Changes the input file schema to an easily readable and understanble form that was used to implement the constraints of the project.
	
3) parsing.asp - Contains the code for obtaining various values for the number of objects and their type in the system.
	
4) demo.asp - The main file where the code for all the constraints resides.
	
5) description.pdf - The pdf containing the problem statement and description of the system.
  
6) script.py - A python file for easier execution of the program.

----------------------------------------------------------------------------

Instructions to Run:

1. Make sure you have python and clingo configured on the system.
2. Copy all these files into your clingo folder/directory (where we have all the txt/asp files to run in clingo).
4. In the terminal (where you run the clingo commands), run the command "python script.py" to test the project.
5. It will then ask which instance you want to run. Choose the number of instance (1, 2, 3, 4, 5).
6. Output will be displayed.

Here are the entire outputs for all the instances (as these cannot be put in the report):

1) Instance 1 -

clingo version 5.4.0
Reading from demo.asp ...
Solving...
Answer: 1
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(0,-1),1) occurs(object(robot,2),move(1,0),2) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),move(0,1),5) occurs(object(robot,1),move(0,-1),6) occurs(object(robot,2),move(0,-1),7) occurs(object(robot,1),move(0,1),8) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,6) occurs(object(robot,1),pickup,7) occurs(object(robot,2),putdown,4) occurs(object(robot,1),putdown,5) occurs(object(robot,2),deliver(2,2,1),3) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(3,4,1),8) occurs(object(robot,1),deliver(1,3,4),9) timeTaken(9) numActions(19)
Optimization: 64
OPTIMUM FOUND

Models       : 1
  Optimum    : yes
Optimization : 64
Calls        : 1
Time         : 0.363s (Solving: 0.24s 1st Model: 0.03s Unsat: 0.20s)
CPU Time     : 0.281s

2) Instance 2 -

clingo version 5.4.0
Reading from demo.asp ...
Solving...
Answer: 1
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(0,-1),1) occurs(object(robot,2),move(1,0),2) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(0,1),5) occurs(object(robot,1),move(0,-1),6) occurs(object(robot,1),move(0,-1),7) occurs(object(robot,2),move(-1,0),7) occurs(object(robot,1),move(-1,0),8) occurs(object(robot,2),move(-1,0),8) occurs(object(robot,2),move(0,1),9) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(2,2,1),3) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(1,3,2),10) timeTaken(10) numActions(20)
Optimization: 75
Answer: 2
occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(0,-1),1) occurs(object(robot,1),move(-1,0),2) occurs(object(robot,2),move(1,0),2) occurs(object(robot,1),move(-1,0),4) occurs(object(robot,2),move(0,1),5) occurs(object(robot,1),move(1,0),6) occurs(object(robot,2),move(-1,0),7) occurs(object(robot,1),move(0,1),8) occurs(object(robot,2),move(0,1),8) occurs(object(robot,2),move(-1,0),9) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,3) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(2,2,1),3) occurs(object(robot,1),deliver(1,1,1),5) occurs(object(robot,2),deliver(1,3,2),10) timeTaken(10) numActions(18)
Optimization: 73
Answer: 3
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),2) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(0,1),5) occurs(object(robot,2),move(-1,0),7) occurs(object(robot,2),move(-1,0),8) occurs(object(robot,2),move(0,1),9) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(2,2,1),3) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(1,3,2),10) timeTaken(10) numActions(17)
Optimization: 72
OPTIMUM FOUND

Models       : 3
  Optimum    : yes
Optimization : 72
Calls        : 1
Time         : 0.598s (Solving: 0.50s 1st Model: 0.03s Unsat: 0.33s)
CPU Time     : 0.672s

3) Instance 3 -

clingo version 5.4.0
Reading from demo.asp ...
Solving...
Answer: 1
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,1),2) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),move(0,-1),6) occurs(object(robot,2),move(0,-1),6) occurs(object(robot,1),move(0,1),8) occurs(object(robot,2),move(-1,0),8) occurs(object(robot,2),pickup,3) occurs(object(robot,1),pickup,4) occurs(object(robot,1),deliver(1,2,1),7) occurs(object(robot,2),deliver(2,4,1),9) timeTaken(9) numActions(16)
Optimization: 61
Answer: 2
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),2) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),move(0,-1),6) occurs(object(robot,2),move(0,-1),6) occurs(object(robot,1),move(1,0),8) occurs(object(robot,2),move(0,1),8) occurs(object(robot,2),pickup,3) occurs(object(robot,1),pickup,4) occurs(object(robot,2),deliver(1,2,1),7) occurs(object(robot,1),deliver(2,4,1),9) timeTaken(9) numActions(14)
Optimization: 59
Answer: 3
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(0,1),6) occurs(object(robot,1),move(0,-1),7) occurs(object(robot,2),move(0,-1),7) occurs(object(robot,1),move(1,0),8) occurs(object(robot,2),move(1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(8) numActions(16)
Optimization: 56
Answer: 4
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),move(0,1),7) occurs(object(robot,1),move(-1,0),8) occurs(object(robot,2),move(0,-1),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(8) numActions(16)
Optimization: 55
Answer: 5
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),move(0,1),7) occurs(object(robot,2),move(0,-1),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(8) numActions(15)
Optimization: 54
Answer: 6
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(0,1),5) occurs(object(robot,1),move(1,0),6) occurs(object(robot,2),move(1,0),6) occurs(object(robot,2),move(0,-1),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(8) numActions(15)
Optimization: 53
Answer: 7
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(0,1),5) occurs(object(robot,2),move(0,-1),6) occurs(object(robot,2),move(1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(8) numActions(14)
Optimization: 52
Answer: 8
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,1),move(0,1),6) occurs(object(robot,2),move(1,0),6) occurs(object(robot,2),move(0,-1),7) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),8) timeTaken(8) numActions(15)
Optimization: 51
Answer: 9
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(1,0),3) occurs(object(robot,1),move(0,1),5) occurs(object(robot,2),move(0,-1),6) occurs(object(robot,2),move(1,0),7) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,2),putdown,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),8) timeTaken(8) numActions(14)
Optimization: 50
Answer: 10
occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(0,-1),2) occurs(object(robot,1),move(0,-1),4) occurs(object(robot,2),move(0,-1),4) occurs(object(robot,1),move(1,0),8) occurs(object(robot,2),move(1,0),8) occurs(object(robot,2),pickup,2) occurs(object(robot,1),pickup,3) occurs(object(robot,1),deliver(2,4,1),6) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 43
Answer: 11
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),2) occurs(object(robot,1),move(0,-1),4) occurs(object(robot,2),move(0,-1),4) occurs(object(robot,1),move(1,0),8) occurs(object(robot,2),move(1,0),8) occurs(object(robot,2),pickup,2) occurs(object(robot,1),pickup,3) occurs(object(robot,1),deliver(2,4,1),6) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 42
Answer: 12
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(0,-1),4) occurs(object(robot,2),move(0,-1),4) occurs(object(robot,1),move(0,1),8) occurs(object(robot,2),move(1,0),8) occurs(object(robot,1),pickup,3) occurs(object(robot,2),pickup,3) occurs(object(robot,1),deliver(2,4,1),6) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 41
Answer: 13
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),4) occurs(object(robot,2),move(0,-1),4) occurs(object(robot,1),move(0,1),7) occurs(object(robot,2),move(1,0),7) occurs(object(robot,1),pickup,3) occurs(object(robot,2),pickup,3) occurs(object(robot,1),deliver(2,4,1),6) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 40
Answer: 14
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),4) occurs(object(robot,2),move(0,-1),4) occurs(object(robot,1),move(1,0),7) occurs(object(robot,2),move(1,0),7) occurs(object(robot,1),pickup,3) occurs(object(robot,2),pickup,3) occurs(object(robot,1),deliver(2,4,1),6) occurs(object(robot,2),deliver(1,2,1),8) timeTaken(6) numActions(10)
Optimization: 39
Answer: 15
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(0,1),8) occurs(object(robot,2),move(1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 37
Answer: 16
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(0,1),7) occurs(object(robot,2),move(1,0),7) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 36
Answer: 17
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(0,1),7) occurs(object(robot,2),move(1,0),7) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),8) timeTaken(6) numActions(10)
Optimization: 35
Answer: 18
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(0,-1),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),9) timeTaken(6) numActions(10)
Optimization: 34
Answer: 19
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(0,1),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),8) timeTaken(6) numActions(10)
Optimization: 33
Answer: 20
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(0,1),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),move(-1,0),6) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),6) timeTaken(6) numActions(11)
Optimization: 32
Answer: 21
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(0,-1),3) occurs(object(robot,2),move(0,-1),3) occurs(object(robot,1),move(0,1),5) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,2) occurs(object(robot,1),deliver(2,4,1),4) occurs(object(robot,2),deliver(1,2,1),6) timeTaken(6) numActions(10)
Optimization: 31
OPTIMUM FOUND

Models       : 21
  Optimum    : yes
Optimization : 31
Calls        : 1
Time         : 0.189s (Solving: 0.14s 1st Model: 0.02s Unsat: 0.09s)
CPU Time     : 0.141s

4) Instance 4 -

clingo version 5.4.0
Reading from demo.asp ...
Solving...
Answer: 1
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),2) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),deliver(3,2,1),3) occurs(object(robot,2),deliver(3,2,1),5) occurs(object(robot,1),deliver(1,1,1),9) occurs(object(robot,2),deliver(2,2,1),9) timeTaken(5) numActions(11)
Optimization: 31
Answer: 2
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),2) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),deliver(3,2,1),3) occurs(object(robot,2),deliver(3,2,1),4) occurs(object(robot,1),deliver(1,1,1),9) occurs(object(robot,2),deliver(2,2,1),9) timeTaken(5) numActions(11)
Optimization: 30
Answer: 3
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),2) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,4) occurs(object(robot,2),deliver(2,2,1),4) occurs(object(robot,1),deliver(1,1,1),7) occurs(object(robot,2),deliver(3,2,2),7) timeTaken(5) numActions(10)
Optimization: 29
Answer: 4
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),4) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,4) occurs(object(robot,2),deliver(3,2,2),5) occurs(object(robot,1),deliver(1,1,1),7) occurs(object(robot,2),deliver(2,2,1),7) timeTaken(4) numActions(10)
Optimization: 27
Answer: 5
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),2) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),deliver(2,2,1),5) occurs(object(robot,1),deliver(1,1,1),7) occurs(object(robot,2),deliver(3,2,2),7) timeTaken(4) numActions(10)
Optimization: 25
Answer: 6
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(1,0),1) occurs(object(robot,2),move(0,-1),2) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),pickup,0) occurs(object(robot,1),pickup,2) occurs(object(robot,2),deliver(2,2,1),3) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(3,2,2),4) timeTaken(4) numActions(10)
Optimization: 20
OPTIMUM FOUND

Models       : 6
  Optimum    : yes
Optimization : 20
Calls        : 1
Time         : 0.268s (Solving: 0.17s 1st Model: 0.02s Unsat: 0.09s)
CPU Time     : 0.234s

5) Instance 5 -

clingo version 5.4.0
Reading from demo.asp ...
Solving...
Answer: 1
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,2),move(1,0),5) occurs(object(robot,1),move(-1,0),6) occurs(object(robot,2),move(0,1),6) occurs(object(robot,1),move(-1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,1),pickup,7) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,1),deliver(1,1,1),9) timeTaken(9) numActions(12)
Optimization: 57
Answer: 2
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,1),move(0,1),3) occurs(object(robot,2),move(1,0),6) occurs(object(robot,2),move(-1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,2),pickup,7) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,2),deliver(1,1,1),9) timeTaken(8) numActions(11)
Optimization: 51
Answer: 3
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,1),move(0,1),3) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),move(-1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,2),pickup,7) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,2),deliver(1,1,1),9) timeTaken(8) numActions(11)
Optimization: 50
Answer: 4
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,1),move(0,1),3) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),move(-1,0),8) occurs(object(robot,2),pickup,1) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,2),deliver(1,1,1),9) timeTaken(8) numActions(11)
Optimization: 49
Answer: 5
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,1),move(0,1),3) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),move(-1,0),7) occurs(object(robot,2),pickup,1) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,2),deliver(1,1,1),9) timeTaken(8) numActions(11)
Optimization: 48
Answer: 6
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,1),move(0,1),3) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),move(-1,0),7) occurs(object(robot,2),pickup,1) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,2),deliver(1,1,1),8) timeTaken(8) numActions(11)
Optimization: 47
Answer: 7
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,2),move(-1,0),0) occurs(object(robot,2),move(0,1),2) occurs(object(robot,2),move(1,0),5) occurs(object(robot,2),move(-1,0),7) occurs(object(robot,2),pickup,1) occurs(object(robot,2),pickup,6) occurs(object(robot,2),putdown,4) occurs(object(robot,2),deliver(1,3,4),3) occurs(object(robot,2),deliver(1,1,1),8) timeTaken(8) numActions(10)
Optimization: 46
Answer: 8
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),4) occurs(object(robot,2),move(-1,0),4) occurs(object(robot,1),move(1,0),7) occurs(object(robot,2),move(0,1),7) occurs(object(robot,1),pickup,3) occurs(object(robot,2),pickup,6) occurs(object(robot,1),putdown,6) occurs(object(robot,1),deliver(1,1,1),5) occurs(object(robot,2),deliver(1,3,4),8) timeTaken(7) numActions(11)
Optimization: 45
Answer: 9
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(-1,0),1) occurs(object(robot,2),move(1,0),4) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,2),move(-1,0),5) occurs(object(robot,1),move(0,1),7) occurs(object(robot,2),move(0,1),7) occurs(object(robot,1),pickup,4) occurs(object(robot,2),pickup,6) occurs(object(robot,1),deliver(1,1,1),6) occurs(object(robot,2),deliver(1,3,4),9) timeTaken(6) numActions(12)
Optimization: 44
Answer: 10
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,2),move(-1,0),5) occurs(object(robot,1),move(0,1),7) occurs(object(robot,2),move(0,1),7) occurs(object(robot,1),pickup,4) occurs(object(robot,2),pickup,6) occurs(object(robot,1),deliver(1,1,1),6) occurs(object(robot,2),deliver(1,3,4),9) timeTaken(6) numActions(10)
Optimization: 42
Answer: 11
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),5) occurs(object(robot,2),move(-1,0),5) occurs(object(robot,1),move(1,0),7) occurs(object(robot,2),move(0,1),7) occurs(object(robot,1),pickup,4) occurs(object(robot,2),pickup,6) occurs(object(robot,1),deliver(1,1,1),6) occurs(object(robot,2),deliver(1,3,4),8) timeTaken(6) numActions(10)
Optimization: 41
Answer: 12
occurs(object(robot,1),move(0,-1),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,2),move(0,1),1) occurs(object(robot,1),move(-1,0),2) occurs(object(robot,1),move(-1,0),4) occurs(object(robot,2),move(-1,0),4) occurs(object(robot,1),move(0,1),6) occurs(object(robot,2),move(0,1),6) occurs(object(robot,2),pickup,2) occurs(object(robot,1),pickup,5) occurs(object(robot,2),deliver(1,1,1),5) occurs(object(robot,1),deliver(1,3,4),7) timeTaken(6) numActions(12)
Optimization: 37
Answer: 13
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),move(-1,0),3) occurs(object(robot,1),move(1,0),6) occurs(object(robot,2),move(0,1),6) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,5) occurs(object(robot,1),putdown,7) occurs(object(robot,1),deliver(1,1,1),5) occurs(object(robot,2),deliver(1,3,4),7) timeTaken(6) numActions(11)
Optimization: 35
Answer: 14
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),move(-1,0),3) occurs(object(robot,1),move(1,0),6) occurs(object(robot,2),move(0,1),6) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,5) occurs(object(robot,1),deliver(1,1,1),5) occurs(object(robot,2),deliver(1,3,4),7) timeTaken(6) numActions(10)
Optimization: 34
Answer: 15
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),move(-1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(0,1),5) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,1),putdown,7) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(1,3,4),7) timeTaken(6) numActions(11)
Optimization: 33
Answer: 16
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),move(-1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(0,1),5) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(1,3,4),7) timeTaken(6) numActions(10)
Optimization: 32
Answer: 17
occurs(object(robot,1),move(-1,0),0) occurs(object(robot,1),move(-1,0),1) occurs(object(robot,1),move(-1,0),3) occurs(object(robot,2),move(-1,0),3) occurs(object(robot,1),move(1,0),5) occurs(object(robot,2),move(0,1),5) occurs(object(robot,1),pickup,2) occurs(object(robot,2),pickup,4) occurs(object(robot,1),deliver(1,1,1),4) occurs(object(robot,2),deliver(1,3,4),6) timeTaken(6) numActions(10)
Optimization: 31
OPTIMUM FOUND

Models       : 17
  Optimum    : yes
Optimization : 31
Calls        : 1
Time         : 0.299s (Solving: 0.22s 1st Model: 0.01s Unsat: 0.01s)
CPU Time     : 0.297s

****************************************************** END ********************************************************************
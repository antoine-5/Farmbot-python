# Farmbot-python

You can find here a planning the farmbot executes completely

# Files explanation

- **newfileplanning.py** generates the domain.pddl file and the problem.pddl file (easier way to write pddl files using python language) with cmd: ***python -m py2pddl.parse newfileplanning.py***
- **execute.txt** is the classical planning generated by the ff solver using the domain.pddl file and the problem.pddl file with cmd: ***./ff -o domain.pddl -f problem.pddl >execute.txt***
- **torobot.py** file contains the file that should be sent to the robot so it executes everything
- **commands.txt** contains the saved vector containing all the cmds that will be executed by the robot using the torobot.py file

# How to run the code

In short the user should 
1. run the new.file.planning.py to create the 2 pddls files
2. run the ff solver to generate the classical planning and put the result in execute.txt
3. run the plan02.py file to parse the classical planning which will sqve the result in commands.txt
4. run the torobot.py file which will run the robot.


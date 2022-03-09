Written by: Matthew Rezkalla
Date: 2022-02-18
Description: ReadMe file regarding the EnvironmentController, Observation, Results, and RewardCalculator.

All files located in the Shared folder. 

EnvironmentController.py - 
Containing access and control over CybORG envornment. This class creates the CybORG environment, initiates the variables for agents, 
actions, rewards, results, and observations. Functions enable this file to create agents and scenarios,
check if the goal has been reached, take steps forward, observe those actions, results, reset, pause, and shutdown environment.


Observation.py - 
Creates and stores a dictionary of information regarding the environment, agent, action-observation pairs. The information
stored relates to PC information like IP address and other processes, alongside information for the simulated environment and what is happening within it. 


Results.py - 
Works closely with the Observation class. Initializes and holds information regarding the state, action, observation, reward, and error status. 
Functions keep track of errors that happen and enables external sources to copy the information regarding the current action-observation, 
as well as printing the results. 


RewardCalculator.py - 
A base class for the RedRewardCalculator.py and BlueRewardCalculator.py. The class initiallizes agent name, state, and observation. Functions enable it to
reset and calculate reward. Calculating rewards take place in the Red or Blue calculator. Different reward levels are calculated based on the type of agent. 


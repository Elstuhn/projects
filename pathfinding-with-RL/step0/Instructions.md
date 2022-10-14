# Introduction
### Hello welcome to the first step of your reinforcement learning project. The first thing you need to do for every RL project is to create the environment
### You will have to make an environment (make it a class) and introduce the correct variables.

## Variables
- height and width of environment/map
- starting position (x, y) of agent
- destination/end coordinates (x,y)
- list of actions (can be number coded)
**Feel free to introduce any other variable you deem necessary!**

## Method
- **Reset method**
 
  The reset method has to reset the current position of your agent and set the status of whether training is done or not to False
  
- **Step method**

  This method should take in an action and change the current state based on that action, it should return the next state and the reward of the new state

- **Random action method**

  This method should return a random action from your list of actions 

- **Render method (optional)**

  You can make a render method that shows the map and where the agent is currently at just to show the path it took

# Supplementary Information

## Equation Used In The Project (You can use your own if you want)

### Terms 
**To understand what you're going to see, you'll need to understand some of the equations, symbols and functions**
- s' is the state you end up in after taking action a in state s
- r is the reward function, it tells you what the reward is for taking an action in a certain state
- Q is the value function which returns the reward for taking a certain action in a certain state
- V is the value of a state which is the expected total reward we can get starting in that state


### Greedy Policy
<img width="285" alt="image" src="https://user-images.githubusercontent.com/66341506/194858672-68867d4a-25e3-4248-aea9-b27c25e3422e.png">
<img width="345" alt="image" src="https://user-images.githubusercontent.com/66341506/194858708-82237429-9c8b-4309-a7b2-24bb21820bea.png">

**Greedy Policy In Code**

<img width="283" alt="image" src="https://user-images.githubusercontent.com/66341506/197928945-e1801be5-77ae-4e0b-8669-4f754059ae38.png">


### The Bellman Equation
<img width="447" alt="image" src="https://user-images.githubusercontent.com/66341506/194855286-e22e9ecf-3037-4e07-a1d2-c14c39d2b998.png">

**Updating qtable values with the Bellman Equation**

<img width="338" alt="image" src="https://user-images.githubusercontent.com/66341506/194863963-fb3b3d6b-2e35-4f30-8093-36f8116145a9.png">

### Balancing Exploration and Exploitation
**Of course we want to promote exploraton in our agent so that the agent can explore every possible move to know which is the best one**

**To do this, we introduce two new variables, Epsilon and Decay**

**Epsilon is the threshold to take a random action, if we generate a random number below the epsilon value, we execute a random action**

<img width="211" alt="image" src="https://user-images.githubusercontent.com/66341506/195113662-05a5f153-ec5a-46d0-b3ab-50ef71478515.png">

**As you explore more options and get further into training, you want to slowly stop exploring and start exploiting more so you introduce decay to slowly reduce the value of epsilon to make the threshold lesser**

<img width="157" alt="image" src="https://user-images.githubusercontent.com/66341506/195113923-f9c0054d-dd88-4a29-8c57-9b4184af3467.png">

##### Notes
- Gamma is a discount factor, it balances out immediate and future rewards. Read more about it [here](https://towardsdatascience.com/practical-reinforcement-learning-02-getting-started-with-q-learning-582f63e4acd9#:~:text=gamma%20is%20the%20discount%20factor,varies%20from%200%20to%201.)

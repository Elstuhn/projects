# Time for you to code the main logic of the program!

1. First at the start of every epoch you have to restart your state
2. Make another loop for while the agent has not reached the end yet
3. In that loop, code your logic for choosing an action (logic for random action or greedy policy)
4. After defining your action, put it into your environment's step method and get the next state, reward and status of done from that
5. Update your qtable using the bellman equation 
6. Set your current state as the next state returned by the environment's step method
7. If the status of done is 1, the while loop will be terminated
8. Decrease epsilon by the product of both epsilon and decay

### That's all there is to it! Now your agent can traverse your map!

# Note That This Is Only A Template! Not Everything Is Filled And You Will Have To Code Most Parts By Yourself!

## Environment
```python
import numpy as np

class Env:
    def __init__(self):
        self.height = 
        self.width = 
        self.posX = 
        self.posY = 
        self.endX = 
        self.endY = 
        self.actions = []
        self.stateCount = self.height*self.width
        self.actionCount = len(self.actions)
        
    def reset(self):
        self.posX = 
        self.posY = 
        self.done = 
        return 
    
    def step(self, action):
        if not action: # left
            self.posX = self.posX - 1 if self.posX > 0 else self.posX
        if action == 1: # right
            self.posX = self.posX + 1 if self.posX < self.width - 1 else self.posX
        if action == 2: # up
            self.posY = self.posY - 1 if self.posY > 0 else self.posY
        if action == 3: # down
            self.posY = self.posY + 1 if self.posY < self.height - 1 else self.posY
            
        nextState = self.width*self.posY + self.posX
        return nextState, reward, done 
    
    def randomAction(self):
        return
    
    def render(self):
        for i in range(self.height):
            for j in range(self.width):
                if self.posY == i and self.posX == j:
                    print("O", end='')
                elif self.endY == i and self.endX == j:
                    print("T", end='')
                else:
                    print(".", end='')
            print("")
```


## Main
```py
from env import Env
import numpy as np
import time 
import os 


env = Env()
qtable = np.random.rand(env.stateCount, env.actionCount).tolist()

epochs = 
gamma = 
epsilon = 
decay = 

for i in range(epochs):
    state, reward, done = 
    print(f"Epoch #{i+1}")
    time.sleep(1)
    while not done:
        env.render()
        time.sleep(0.005)
        
        if :
            action = env.randomAction()
        else:
            action = 
        
        next_state, reward, done =
        qtable[state][action] = 
        state = 
        
    epsilon -= 
        
    time.sleep(0.8)
```

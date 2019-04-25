# Report for Udacity DRLND Project 1 - Navigation

## Learning Algorithm

To solve this project I utilized the Deep Q-Network from the OpenAI Gym's LunarLander-v2 DQN exercise solution (https://github.com/udacity/deep-reinforcement-learning/tree/master/dqn/solution). I modified the definition of the function `dqn` in `Deep_Q_Network_Solution.ipynb` to interact with the Bananas environment, but left `dqn_agent.py` and `model.py` unchanged. I had intended to use this as a starting point and then modify the neural network architecture and hyperparameters to solve this new environment, but found that the default values carried over from the Lunar Lander exercise already solved the Bananas environment in only 318 episodes.

### Hyperparameters

 - Maximum number of episodes: 2000
 - Maximum number of steps per episode: 1000
 - Epsilon starting value: 1.0
 - Epsilon minimum value: 0.01
 - Epsilon decay rate: 0.995
 - Replay buffer size: 10,000
 - Minibatch size: 64
 - Discount factor (gamma): 0.99
 - Soft update factor (tau): 0.001
 - Learning rate: 5e-4
 - Target network update frequency: 4

### Network Architecture

 - Fully Connected Layer 1:
   - Inputs: 37
   - Outputs: 64
   - Activation: ReLU
 - Fully Connected Layer 2:
   - Inputs: 64
   - Outputs: 64
   - Activation: ReLU
 - Fully Connected Layer 3:
   - Inputs: 64
   - Outputs: 4
   - Acitvation: Linear

## Plot of Rewards

**Insert plot figure**

On the first try (plot above), the agent solved this environment in **318 episodes**. Out of curiosity, I reran the training process two more times, which were solved in 353 and 774 episodes. So while 318 was a lucky first run, the agent does train quickly consistently.

## Ideas for Future Work

Since it was not necessary to tune any hyperpameters or the model architecture in order to solve this problem, there is very likely opportunity to improve the agent's performance by experimenting with these. Alternative training algorithms, such as dueling DQN, could also lead to a better agent. The saved agent here was also stopped short of reaching optimal performance, since the goal was to report the number of epochs to reach an average score higher than 13. By letting the current agent train for longer, the agent's test performance is certain to improve.

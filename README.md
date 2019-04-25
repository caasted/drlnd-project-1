[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Udacity DRLND Project 1 - Navigation

## Project Details

In this project, I trained a reinforcement learning agent to navigate and collect bananas in a large, square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of the agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction.  Given this information, the agent learned how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, the agent attained an average score of +13 over 100 consecutive episodes.

## Getting Started

### Installing Dependencies

This project is from the Udacity DRLND repository and requires all of the dependencies listed at https://github.com/udacity/deep-reinforcement-learning#dependencies are satisfied in order to execute the code.

### Download the Unity Environment

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

2. Place the file in your clone of this repository, in the root of the `drlnd-project-1` folder, and unzip (or decompress) the file. 

## Instructions

The entry point for this application is the Jupyter Notebook `Navigation.ipynb`.
 1. Launch a jupyter notebook service in `drlnd-project-1` and open `Navigation.ipynb`.
 2. Edit cell #2 (`env = UnityEnvironment(file_name="Banana_Linux/Banana.x86_64")`) based on the instructions above it to match your version of the Unity Environment.
 3. To execute all of the code and train a new agent, click `Cell` --> `Run All`.
 4. To view the pre-trained agent, execute all of the cells except cell 10, which starts with `scores = dqn()`.

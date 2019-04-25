# Udacity DRLND Project 1 - Navigation

## Installing Dependencies

This project is from the Udacity DRLND repository and requires all of the dependencies listed at https://github.com/udacity/deep-reinforcement-learning#dependencies are satisfied in order to execute the code.

## Download the Unity Environment

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

2. Place the file in your clone of this repository, in the root of the `drlnd-project-1` folder, and unzip (or decompress) the file. 

## Running the Code

The entry point for this application is the Jupyter Notebook `Navigation.ipynb`. Launch a jupyter notebook service in `drlnd-project-1` and open `Navigation.ipynb`. Edit cell #2 (`env = UnityEnvironment(file_name="Banana_Linux/Banana.x86_64")`) based on the instructions above it to match your version of the Unity Environment. Click `Cell` --> `Run All` to execute the code and train a new agent.

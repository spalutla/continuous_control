# Project 2: Continuous Control
This Repo consists of Udacity's DRLND project2

## Project Environment and Dependencies
The code is written in Python3 and PyTorch.  Unityagents package has the problem environment, described in the section below.
Dependencies are specified in the requirements file and can be installed by:
```
pip install -r requirements.txt
```

## RL Problem Environment
This project uses Reacher environment, from Unity.

![Alt Text](https://s3.amazonaws.com/video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif)

In this environment, a double-jointed arm can move to target locations. A reward of +0.1 is provided for each step that the agent's hand is in the goal location. Thus, the goal of your agent is to maintain its position at the target location for as many time steps as possible.

The observation space consists of 33 variables corresponding to position, rotation, velocity, and angular velocities of the arm. Each action is a vector with four numbers, corresponding to torque applicable to two joints. Every entry in the action vector should be a number between -1 and 1.

## Training the Agent
The individual cells in notebook ```Continuous_Control.ipynb``` can be executed sequentially to train the agent. Note that after training, this file saves the actor and critic NN weigths in the checkpoint.pth files.  Additionally, note that these files are provided in the git repo and a re-run will cause these files to be generated with the new run.

If you just want to see the performance, the use the ```Saved_Agent.ipynb```. Execute the only cell in the notebook.  The code loads the actor and critic NN weights and runs the environment for 200 time steps before terminating.

[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Banana Navigation

### Introduction

This project implements Agents with DQN and DDQN algorithms to navigate (and collect bananas!) in a large, square world.  

![Trained Agent][image1]

A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana.  Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.  

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction.  Given this information, the agent has to learn how to best select actions.  Four discrete actions are available, corresponding to:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic, and in order to solve the environment, your agent must get an average score of +13 over 100 consecutive episodes.

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

2. Place the file in the BananaNav GitHub repository and unzip (or decompress) the file. 

### Instructions

1. Before you can start with the rest of the project please ensure that you have [Anaconda](https://docs.anaconda.com/anaconda/install/) installed. Please follow instructions that apply to your OS in this [link](https://docs.anaconda.com/anaconda/install/).

2. Create and activate a new environment with Python 3.6
    * **Linux and Mac**
    
         ```` 
          conda create --name dqn python=3.6
          conda activate dqn
   * **Windows**
        ````
        conda create --name dqn python=3.6
        activate dqn
 3. Make sure to run the following command inside the folder `banana-unity-nav-rl`
    ````
    pip install -r requirements.txt
 4. Once all the dependencies have been installed start up the jupyter notebook by running the command and following the link provided in the console.
    ````
    jupyter-notebook

5. Follow the instructions in `Navigation.ipynb` to get started with training a DQN agent on the Banana Environment!  

6. To get started on training the DDQN agent follow the instructions in `Navigation-DDQN.ipynb`
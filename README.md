# Udacity-DRL-Bananas
DRL algorithm trained on the Banana pick up game of AI gym

This reportory contains files used to build a deep reinforcement learning network to solve the Bananas collector game. An agent must pick up yellow bananas but not blue bananas. 

### Banana Game collector description
the state space is a vector of 37 dimensions that describe the environment where the agent is. The action space consist of 4 possible moves(up,down,right left). the reward is +1 for picking up a yellow banana and -1 for picking up a blue banana

to be defined as successful the agent must obtain a score of at least 13 over an average of 100 episodes

### Description of files used

the 4 files below are used to build & train the models and have dependencies from Pytorch, Numpy, namedTuples,UnityEnvironment,Gym and Collections.

1. DRL Bananas v01.pth : A trained DRL model that obtains an average score of at least 13 on 100 consecutive episodes

2. Model.py :A Deep neural network, fully connected with 2 hidden layers each containing 64 nodes. 
    1. the forward method overrides the nn.module forward method as prescribed in the documentation
    2. the forward method does not need to be called explicitly

3. dqn_agent.py: An agent class that implements the Google Deepmind learning with experience replay algorithm and a ReplayBuffer class that implements the memory methods required for experience replay. Agent class inherits the Qnetwork class in Model.py
   
4. DRL Udacity Bananas.ipynb: A jupyter notebook  that connects to Unity environment to run the /Banana_Linux_NoVis/Banana.x86_64 assignment. the notebook contains the function dqn which is used to train a DRL network using the state,actions,reward as inputs.

5. DRL report: a small report describing the vanilla DRL model used to complete this assigmnent along potential improvements

### How to run the model

Everything is self contained in the DRL Udacity Bananas.ipynb notebook. Simply run every cell and the *dqn* function will create a trained model as an ouput in the directory. Simply change the name of the output file in the *dqn* function to save a new copy

### How to set up the dependencies



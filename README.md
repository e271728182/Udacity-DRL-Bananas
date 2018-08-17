# Udacity-DRL-Bananas
DRL algorithm trained on the Banana pick up game of AI gym

This reportory contains files used to build a deep reinforcement learning network to solve the Bananas collector game. An agent must pick up yellow bananas but not blue bananas. to be defined as successful the agent must obtain a score of at least 13 over an average of 100 episodes

the 4 files below are used to build & train the models and have dependencies from Pytorch, Numpy, namedTuples,UnityEnvironment,Gym and Collections.

1.DRL Bananas v01.pth : A trained DRL model that obtains an average score of at least 13 on 100 consecutive episodes

2.Model.py :A Deep neural network, fully connected with 2 hidden layers each containing 64 nodes. 
  the forward method overrides the nn.module forward method as prescribed in the documentation
  the forward method does not need to be called explicitly

3. dqn_agent.py: An agent class that implements the Google Deepmind learning with experience replay algorithm and a ReplayBuffer class that implements the memory methods required for experience replay. Agent class inherits the Qnetwork class in Model.py
   
4.DRL Udacity Bananas.ipynb: A jupyter notebook  that connects to Unity environment to run the /Banana_Linux_NoVis/Banana.x86_64 assignment. the notebook contains the function dqn which is used to train a DRL network using the state,actions,reward as inputs.

5. DRL report: a small report describing the vanilla DRL model used to complete this assigmnent along potential improvements

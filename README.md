# Udacity-DRL-Bananas
DRL algorithm trained on the Banana pick up game of AI gym

the 4 files below have dependencies from Pytorch, Numpy, namedTuples,UnityEnvironment,Gym and Collections

1.DRL Bananas v01.pth : A trained DRL model that obtains an average score of at least 13 on 100 consecutive episodes

2.Model.py :A Deep neural network, fully connected with 2 hidden layers each containing 64 nodes. 
  the forward method overrides the nn.module forward method as prescribed in the documentation
  the forward method does not need to be called explicitly

3. dqn_agent.py: An agent class that implements the Google Deepmind learning with experience replay algorithm and a ReplayBuffer class that implements the memory methods required for experience replay. Agent class inherits the Qnetwork class in Model.py
   

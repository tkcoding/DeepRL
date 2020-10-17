# Deep Reinforcement Learning on banana collector

Using Unity ML-Agents. 
[link to banana collector!](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector)

For this project, agent will be trained to navigate and collect bananas in a sqare world.

Reward as follows:
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. 

Objective of agent:
Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

State space in the environment:
Number of state space : 37
Vector of state space type : continuous
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. 

Example of state space :
[ 1.          0.          0.          0.          0.84408134  0.          0.
  1.          0.          0.0748472   0.          1.          0.          0.
  0.25755     1.          0.          0.          0.          0.74177343
  0.          1.          0.          0.          0.25854847  0.          0.
  1.          0.          0.09355672  0.          1.          0.          0.
  0.31969345  0.          0.        ]

Action space:
Number of action space : 4
0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right


Completion of successful agent:
The task is episodic, and in order to solve the environment, agent must get an average score of +13 over 100 consecutive episodes.

Packages required:
unityagents (refer to :https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md)


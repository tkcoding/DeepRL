# Deep Reinforcement Learning on banana collector

## Introduction to banana collector navigation using DQN/Double DQN
Using Unity ML-Agents. 
[link to banana collector!](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector)
![DQN agent](assets/BananaCollector.png)

For this project, agent will be trained to navigate and collect bananas in a sqare world.

Reward as follows:
A reward of +1 is provided for collecting a yellow banana, and a reward of -1 is provided for collecting a blue banana. 

Objective of agent:
```
Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.
```

State space in the environment:
```
Number of state space : 37
Vector of state space type : continuous
The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around the agent's forward direction. 
```

State space :
__Number of state space : 37__
```
[ 1.          0.          0.          0.          0.84408134  0.          0.    1.          0.          0.0748472   0.          1.          0.          0.]
```

*Action space:*
__Number of action space : 4__
```
0 - move forward.
1 - move backward.
2 - turn left.
3 - turn right
```

Completion of successful agent:
```
The task is episodic, and in order to solve the environment, agent must get an average score of +13 over 100 consecutive episodes.
```

## Content of this repository
* __report.pdf__: a document that describes the details of the different implementation, along with ideas for future work.
* jupyter notebook __Banana_Navigator/Navigation.ipynb__: Notebook to run agent learning at DQN and DDQN with the switch at agent class DDQN=False (DQN) and DDQN=True (DDQN).
* __checkpoint_ddqn.pth__ : Weight file that has the trained agent using DDQN.
* __checkpoint_dqn.pth__ : Weight file that has the trained agent using DQN.
* __requiremets.txt__ : File for dependencies . Can run trhough pip install -r requirements.txt

## Requirements
Create a virtual environment and activate it.

```
python -m venv banana_collector
source banana_collector/bin/activate
```

Install Unity ml-agents.
```
git clone https://github.com/Unity-Technologies/ml-agents.git
git -C ml-agents checkout 0.4.0b
pip install ml-agents/python/.
```

Install the project requirements.

```
pip install -r requirements.txt
```
__Installation of envirnoment for unity__

Installation Guides for unity agent:
unityagents (refer to :https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md)

Installation of required packages:
pip install -r requirements.txt


__Expected result :__
```Deep Q-network rolling standard deviation and rolling mean reward graph```

![DQN reward](assets/DQN_reward.png)


```Double Deep Q-network rolling standard deviation and rolling mean reward graph```

![DDQN reward](assets/DDQN_reward.png)

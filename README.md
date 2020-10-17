# Deep Reinforcement Learning on banana collector

Using Unity ML-Agents. 
[link to banana collector!](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#banana-collector)

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
* __report.pdf__: a document that describes the details of the different implementation, along with ideas for future work
* jupyter notebook __load_run_agent.ipynb__: a notebook that can load and run the saved agents
* folder __double_dqn__: implementation of double deep q network (succeeded)
* folder __dueling_double_dqn__: implementation of double deep q network with a dueling network (succeeded)
* folder __per_dueling_double_dqn__: implementation of an agent with double DQN, dueling Network, and Prioritized Experience Replay all together (pending)
## Requirements
To run the codes, follow the next steps:
* Create a new environment:
	* __Linux__ or __Mac__: 
	```bash
	conda create --name dqn python=3.6
	source activate dqn
	```
	* __Windows__: 
	```bash
	conda create --name dqn python=3.6 
	activate dqn
	```
* Perform a minimal install of OpenAI gym
	* If using __Windows__, 
		* download swig for windows and add it the PATH of windows
		* install Microsoft Visual C++ Build Tools
	* then run these commands
	```bash
	pip install gym
	pip install gym[classic_control]
	pip install gym[box2d]
	```
* Install the dependencies under the folder python/
```bash
	cd python
	pip install .
```
* Create an IPython kernel for the `dqn` environment
```bash
	python -m ipykernel install --user --name dqn --display-name "dqn"
```
* Download the Unity Environment (thanks to Udacity) which matches your operating system
	* [Linux](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
	* [Mac OSX](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
	* [Windows (32-bits)](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
	* [Windows (64 bits)](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

* Start jupyter notebook from the root of this python codes
```bash
jupyter notebook
```
* Once started, change the kernel through the menu `Kernel`>`Change kernel`>`dqn`
* If necessary, inside the ipynb files, change the path to the unity environment appropriately

Installation Guides :
unityagents (refer to :https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md)


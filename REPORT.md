### Instructions

Follow the instructions in `Tennis.ipynb` to get started with training your own agent!

## Algorithm

**MADDPG* (DDPG) is a multi-agent RL algorithm in which the agents can collaborate as well as compete with each other.

- This project repository uses **MADDPG** algorithm to solve Unity's Tennis environment.

- The network architectures used (2 neural networks) is a simple, fully-connected neural network with 2 hidden layers of sizes, 256 and 128 units. Model definition can be found in `model.py` file.

- Hyperparameter values chosen are as follows :

| Hyperparameter | Value |
| -------------- | ------ |
| GAMMA | 0.99 |
| BUFFER_SIZE | 1e6 |
| BATCH_SIZE | 512 |
| TAU | 1e-3 |
| LR_ACTOR | 9e-3 |
| LR_CRITIC | 9e-3 |
| WEIGHT_DECAY_ACTOR | 1e-7 |
| WEIGHT_DECAY_CRITIC | 1e-7 |
| NOISE_START | 0.8 |
| NOISE_END | 0.15 |
| NOISE_REDUCTION | 0.999 |
| HIDDEN_LAYERS | [256, 128] |
| DEVICE | GPU |

## Rewards Plot

Rewards obtained by agent plotted as function of episodes of training is shown below :

![rewards_plot](https://raw.githubusercontent.com/akshaydp1995/Reacher_Environment/master/rewards.png)

Orange line represents a rolling mean of rewards for latest 100 episodes.

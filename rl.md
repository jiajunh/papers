[TOC]

## Classical RL algorithms

**Human-level control through deep reinforcement learning [Deep Q-learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf)**
* Network for Q values, experience replay, seperate target network for stablization (max operation)

**Deep Reinforcement Learning with Double Q-learning [Double Q-learning](https://arxiv.org/pdf/1509.06461)**
* The max operation tends to over-estimate the Q value, use different Q' for target value, empirically just use the Q from several updates before

**Dueling Network Architectures for Deep Reinforcement Learning [Dueling Q-learning](https://arxiv.org/pdf/1511.06581)**
* One network for V values, another for A(advantage value), Q = V+A

**Policy Gradient Methods for Reinforcement Learning with Function Approximation [Policy Gradient](https://proceedings.neurips.cc/paper_files/paper/1999/file/464d828b85b0bed98e80ade0a5c43b0f-Paper.pdf)**
* Vanilla Policy Gradient

**Continuous Control With Depp Reinforcement Learning [DDPG](https://arxiv.org/pdf/1509.02971)**
* Deep PG with critic model, extend DQN on continuous space.

**Trust Region Policy Optimization [TRPO](https://arxiv.org/pdf/1502.05477)**
* Constraint the step with KL-divergence (elegant math)

**Proximal Policy Optimization Algorithms [PPO](https://arxiv.org/pdf/1707.06347)**
* To simplify TRPO computation, constraint the gradient with a coefficient (practically good and simple).

**Soft Actor-Critic Algorithms and Applications [SAC](https://arxiv.org/pdf/1812.05905)**
* Add an entropy term related to policy term allows more stability and scaling. 

**High-Dimensional continuous Control Using Generalized Advantage Estimation [GAE](https://arxiv.org/pdf/1506.02438)**
* Having a trajectory, use a weighted average of the advantages over the trajectory.

**Conservative Q-Learning for Offline Reinforcement Learning [Conservative Q-laerning](https://arxiv.org/pdf/2006.04779)**



## RL with LLM

**DeepSeekMath: Pushing the Limits of Mathematical Reasoning in Open Language Models [Deepseek GRPO](https://arxiv.org/pdf/2402.03300)**
* GRPO just replace the critic model back to average rewards with several samples, as MC. It’s specifically in math tasks, if we only use the result rewards, then no reward models, and MC is good, since not need another critic model, which may introduce some errors.

**DeepScaleR [deepscaler](https://pretty-radio-b75.notion.site/DeepScaleR-Surpassing-O1-Preview-with-a-1-5B-Model-by-Scaling-RL-19681902c1468005bed8ca303013a4e2)**




# reinforcement learning关键概念
 - agent , enviroment, target
 - state, action, reward
 - policy, value function, model

# 基本概念
    - agent: 与环境进行交互的主体
    - enviroment: 与agent进行交互的环境
    - target: agent的目标，agent的行为会影响到target
    - state: agent在环境中的状态
    - action: agent在环境中的行为
    - reward: agent在环境中的行为的反馈
    - policy: agent的策略，agent在某个状态下采取某个行为的概率
    - value function: agent在某个状态下的价值
    - model: agent对环境的模型


# 学习方法
 - model-free, model-based
   - model-free
     - Q-learning
     - sarsa
     - policy gradient
   - model-based: 可以通过模型来预测下一个状态
     - Q-learning
     - sarsa
     - policy gradient
 - 基于概率的方法，基于价值的方法
   - 基于概率的方法（policy-dbase）
     - policy gradient
     - actor-critic
     - DDPG
     - PPO
     - TRPO
     - A3C
     - A2C
     - SAC
   - 基于价值的方法 （value-based）
     - Q-learning
     - sarsa
     - DQN
     - DDPG
     - PPO
     - TRPO
     - A3C
     - A2C
     - SAC
 - 回合更新，单步更新
   - 回合更新：agent在一个多步游戏结束后，更新参数
     - monte carlo learning
     - policy gradient
   - 单步更新：agent在每一步结束后，更新参数
     - Q-learning
     - sarsa
 - On-policy 与  off-policy
   - on-policy: 采样数据的策略与更新参数的策略相同
     - policy gradient
     - actor-critic
     - DDPG
     - PPO
     - TRPO
     - A3C
     - A2C
     - SAC
   - off-policy: 采样数据的策略与更新参数的策略不同
     - Q-learning
     - sarsa
     - DQN
     - DDPG
     - PPO
     - TRPO
     - A3C
     - A2C
     - SAC
 - 基于误差的方法，基于梯度的方法
 - 基于策略的方法，基于价值的方法

# 基于策略的方法
 - policy gradient
 - actor-critic
 - DDPG
 - PPO
 - TRPO
 - A3C
 - A2C
 - SAC

# 基于价值的方法
 - 

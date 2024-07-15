# PPO
一种策略梯度算法 
learning
PPO P8 https://www.bilibili.com/video/BV18H4y167SD?p=9&spm_id_from=pageDriver&vd_source=cf16088b7296d0c8d01e3b00cbd71a9e
首先：
  强化学习的基本要素：环境、智能体、当前环境或智能体的状态、动作等

![1f87d3da8e477ff5defec28332f3c23](https://github.com/oliii20/PPO/assets/101909874/662a7bf9-945d-4f98-ab05-018cc2b15ae2)
![98ba9660d0f059edb533aa016a8d73a](https://github.com/oliii20/PPO/assets/101909874/02981f3e-a1a0-422d-92a6-f8af90f0f635)
![8981ac227b17c1249cb8095fd4c3355](https://github.com/oliii20/PPO/assets/101909874/a5668a23-608f-4ab6-8295-18bdacc0e9e7)
![761d742bb10f3f85774cff4ac2c502f](https://github.com/oliii20/PPO/assets/101909874/a5dcb84f-f231-416d-a8e6-b13de21646ec)
![2803fd64211087f01f8c5963b0e21ef](https://github.com/oliii20/PPO/assets/101909874/a69886eb-5e04-476f-82a5-13f2f87cb601)
![a006ab30951b57eccce19b680f3f3d4](https://github.com/oliii20/PPO/assets/101909874/17b74c12-b8b2-4d89-9473-fc7868023a08)
核心思想：是对一般的策略梯度算法的改进，因为on policy每一批数据（一个回合）迭代一次，训练起来太慢。off policy找一个网络参数的替身，达到同一批数据能够多次训练网络。
组成：一个Actor、critic网络。actor输出最优策略，critic输出value判断网络好坏。

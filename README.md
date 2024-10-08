# DDPG_Two_Joint_Arm
I design a policy to simulate a simplified, two-joint arm that can reach and track a moving target.

## DDPG 
I develop a deep deterministic policy gradient to learn to control a two-joint arm. The arm's state dynamics are described by a differential equation $a = M(q) \ddot{q} + \Gamma(q, \dot{q}){q}$, where $a$ is the action, $q$ is the configuration vector containing the shoulder and elbow angles in that order, $\dot{q}$ and $\ddot{q}$ are the velocity and acceleration. 

## Factoring $Q$
I decompose the action-value function $Q$ into a combination of more basic functions, in the hope that, by exploiting its internal structure, I can improve learning. 

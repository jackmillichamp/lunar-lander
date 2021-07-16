# Solving LunarLander-v2 Using Deep Q-Networks

## Overview
In this project, LunarLander-v2 (LL) was chosen as the reinforcement
learning problem to be solved. The lander initially spawns at the top of the screen and begins to fall with gravity,
until it either crashes or comes to a halt. The agent’s aim is to select actions in such a way that
maximises the total amount of reward it receives within the duration of the episode. To complete
the task however, the agent must be allowed to learn how to control the lander, so that it consistently
finishes on the landing pad without crashing. The task is considered complete when the agent obtains
a mean reward of 200, over 100 consecutive episodes.

## States
Every time step the agent receives an observation from the environment containing eight values, each
corresponding to one of the items in the list below.
![image](https://github.com/jackmillichamp/lunar-lander/blob/main/states.png)

## Actions
The agent must then choose one of the four possible discrete actions listed below.
![image](https://github.com/jackmillichamp/lunar-lander/blob/main/actions.png)

## Rewards
The agent receives a reward of +10 every time one of the lander’s legs touches the ground, as well
as a negative reward for moving away from the landing pad. The agent receives a reward of −0.03
for firing the side engine and −0.3 for firing the main engine. The terminal states are those in
which the landing craft has either crashed (due to landing upside down or too quickly) or has landed
successfully, resulting in rewards of −100 and +100 respectively. Finishing on the landing pad
carries an additional bonus reward of between +100 and +140.

![image](https://github.com/jackmillichamp/lunar-lander/blob/main/rewards_graph.png)

![image](https://github.com/jackmillichamp/lunar-lander/blob/main/epsilon_graph.png)

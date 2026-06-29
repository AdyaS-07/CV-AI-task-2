# CV-AI-task-2

RL RACING CAR USING PPO

A simple autonomous racing car simulation built using Python, Gymnasium, and Stable-Baselines3 (PPO). The project demonstrates how a reinforcement learning (RL) agent interacts with a custom racing environment to navigate a race track while avoiding collisions.

Project Overview:
This project implements a custom racing environment where an AI-controlled car learns to drive on a user-designed race track.
The environment was built from scratch using Gymnasium and trained using the **Proximal Policy Optimization (PPO)** algorithm from Stable-Baselines3.
Although the agent is trained for a limited number of timesteps in this version, the project demonstrates the complete reinforcement learning pipeline, including environment creation, training, testing, and visualization.

Features:
* Custom Gymnasium Environment
* Custom race track using an image
* PPO Reinforcement Learning Agent
* Collision Detection
* Finish Line Detection
* Reward-based Learning
* Environment Rendering
* Learning Curve Visualization
* GIF Generation of Agent Navigation

 ENVIRONMENT:

Observation Space:
  The agent observes:
    * Car X Position
    * Car Y Position
    * Car Orientation (Angle)

Action Space: 
0-forward
1-turn left
2-turn right
3-brake

Reward Function:
Normal step= -0.1 
collision=-100
finish line = +100
A step penalty of -1 is given for every move to discourage unnecessary movement. A large penalty of -100 is given when the agent crashes or goes out of bounds, marking the end of the episode.

REINFORCEMENT LEARNING (RL) ALGORITHM:
The agent is trained using Proximal Policy Optimization (PPO).
Training parameters include:
* Policy: MLP (multilayer perceptron)
* Learning Rate: 0.0003
* Gamma: 0.99
* Total Timesteps: 20,000 (can be increased for improved performance)
  
 RESULTS:
The project demonstrates:
*Car movement within a custom environment
* Wall collision detection
* Goal-reaching behavior
* PPO-based policy learning
* Performance visualization through reward plots
* System uses penalty-based learning where survival is encouraged by minimizing negative rewards rather than maximizing positive rewards.


AUTHOR: Adyasha Sahani

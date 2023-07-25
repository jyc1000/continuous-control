# Continuous control using DDPG
## Project environment
This project utilizes DDPG algorithm to train an agent robot arm to reach a moving target by controlling the torque in its joints.

### State space
- Dimension: 33
- Dimensions of the state space consists of the position, rotation, velocity, and angular velocities of the arm and the location of the target.

### Action space
- Dimensions: 4
- The action space is a vector of four numbers corresponding to the torque of the two joints. The value of each dimension can take on values between [-1,1]
  
### Rewards
- A reward of +0.1 is given each time step that the arm can position itself in the target location.

### Criteria for a solved environment
The agent must receive an average score greater than 30, averaged over consecutive 100 episodes.
In the case of multiple agents interacting with the environment at once, the average of the score over all the agents must satisfy above requirement.

## Getting started

## Instructions for installing dependencies and downloading needed files

## How to run the code
- Run the Continuous_Control.py to train the model
- 
# Report

## Learning algorithm

### Hyperparameters

### Model architecture

## Result and plot of rewards
Environment solved in 15 episodes!	Average Score: 30.23

## Ideas for future work

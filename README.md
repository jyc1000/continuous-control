# Continuous control using DDPG
## Project environment
This project utilizes DDPG algorithm to train an agent robot arm to reach a moving target by controlling the torque in its joints.

### State space
- Number of dimensions: 33
- Dimensions of the state space consists of the position, rotation, velocity, and angular velocities of the arm and the location of the target.

### Action space
- Number of dimensions: 4
- The action space is a vector of four numbers corresponding to the torque of the two joints. The value of each dimension can take on values between [-1,1]
  
### Rewards
- A reward of +0.1 is given each time step that the arm can position itself in the target location.

### Criteria for solved environment
- The agent must receive an average score greater than 30, averaged over consecutive 100 episodes.
- In the case of multiple agents interacting with the environment at once, the average of the score over all the agents must satisfy above requirement.

## Getting started

### Instructions for installing dependencies
Below are the necessary python version and python libraries.
  - python: 3.6
  - tensorflow
  - Pillow
  - matplotlib
  - numpy
  - jupyter
  - pytest
  - docopt
  - pyyaml
  - protobuf: 3.5.2
  - grpcio: 1.11.0
  - pandas
  - scipy
  - ipykernel
  - unityagents: 0.4.0
  - torch: 1.10.2

### How to run the code
- Run the Continuous_Control.py to train the model.
- Set the appropriate address to the Unity environment file corresponding to the correct operating system in the code below.
    - env = UnityEnvironment(file_name='Reacher_Windows_x86_64_multiple/Reacher.exe')
- Set load_model_continue_learning = True to load a pre-trained model and continue training.

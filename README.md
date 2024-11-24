# CartPole RL Dataset

This repository contains code to generate a dataset of state transitions from the CartPole environment, intended for training RL agents or state prediction models.

## Steps
1. Generate a dataset using `scr/generate_dataset.py`.
2. Visualize the dataset with `scr/visualize_dataset.py`. 

## Dataset Format
Each transition in the dataset has the structure:
- `state`: Current state (4-dimensional vector: [cart position(x), cart velocity(v), pole angle(theta), pole angular velocity(ang_theta)]).
- `action`: Action taken (0 = left, 1 = right).
- `reward`: Reward received (typically 1 per step).
- `next_state`: Next state after taking the action.

## Dependencies
Install required libraries:

# Reinforcement Learning: Grid World and Advanced Techniques

This repository contains a comprehensive exploration of reinforcement learning techniques applied to a custom Grid World environment. The project includes implementations of SARSA and N-step Double Q-learning algorithms, as well as advanced visualization techniques for enhancing understanding and engagement.

## Repository Structure

| File Name                                   | Description                                                                                     |
|---------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Grid_World_Environment_Setup.ipynb**      | Defines the Grid World environment with keys, traps, doors, and rewards using Markov Decision Process principles. |
| **SARSA_Implementation_and_Optimization.ipynb** | Implements the SARSA algorithm for policy optimization, including hyperparameter tuning and evaluation. |
| **N_Step_Double_Q_Learning.ipynb**          | Explores N-step Double Q-learning with varying `n` values and compares its performance against SARSA. |
| **Grid_World_Visualization_Bonus.ipynb**    | Bonus visualization for dynamic agent actions, rewards, and penalties in the Grid World environment. |
| **Bonus_Environment_Simulation_Warehouse.ipynb** | Implements an extended warehouse simulation as an additional environment for testing agent behaviors. |

## Highlights

### Grid World Environment
- **Scenario**: Escape Room Challenge
- **Features**: 
  - Keys to unlock doors
  - Traps with penalties
  - Exit portal with rewards
- **Dynamic Visualization**: Tracks the agent’s state, rewards, and movements in real-time.

### SARSA Algorithm
- **On-policy learning**: Updates Q-values based on the current policy.
- **Hyperparameter tuning**: Explored learning rates and epsilon decay to achieve optimal results.
- **Performance**: The agent successfully learned safe and efficient navigation strategies.

### N-step Double Q-Learning
- **Off-policy learning**: Alternates updates between two Q-tables to reduce overestimation bias.
- **N-step returns**: Combines short-term and long-term rewards for better decision-making.
- **Comparison with SARSA**: Demonstrates higher stability and reward optimization.

### Bonus Features
1. **Dynamic Grid Visualization**: Enhanced graphics for agent movements and interactions.
2. **Warehouse Simulation**: A complex environment to test scalability and adaptability of the algorithms.

## Key Results

- **SARSA**:
  - Best Hyperparameters: `α=0.99`, `ϵ_decay=0.99`
  - Average Reward per Episode: 12,000+
  
- **N-step Double Q-Learning**:
  - Best Hyperparameters: `γ=0.99`, `ϵ_decay=0.98`
  - Average Reward per Episode: 13,500+
  - Optimal `n`: 3 (balances performance and convergence speed)

## Visualization and Insights
- **Dynamic Grid Updates**: Displays real-time agent actions, rewards, and penalties.
- **Graphs**:
  - Reward progression over episodes
  - Epsilon decay and policy convergence
  - Q-table updates for different `n` values

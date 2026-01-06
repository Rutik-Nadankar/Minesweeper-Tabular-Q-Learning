# Minesweeper-Tabular-Q-Learning
A Reinforcement Learning–based Minesweeper agent implemented using tabular Q-learning to study decision-making under uncertainty.

### Exploration–Exploitation Strategy
An **ε-greedy policy** is used to balance exploration and exploitation:
- With probability ε, the agent selects a random action
- Otherwise, it selects the action with the highest Q-value
- ε decays over time to encourage exploitation in later training stages

---

## System Architecture
The system consists of the following components:
- Minesweeper environment implemented using **Pygame**
- Q-learning agent
- Training loop for episodic learning
- Evaluation module for performance measurement
- Graphical interface for visual feedback

A modular design ensures separation between environment dynamics, visual rendering, and learning logic.

---

## Experimental Setup
- **Training Episodes:** 8,000  
- **Board Sizes:** Multiple grid configurations  
- **Mine Density:** Varying levels of uncertainty  
- **Evaluation Metric:** Win rate per episode  
- **Baseline Policy:** Random action selection  

---

## Results and Analysis
The trained agent demonstrates a clear improvement over random play. In low-uncertainty configurations, the agent achieves win rates of up to **70%**, while in higher-uncertainty settings, performance drops to approximately **15%**.

These results confirm that tabular Q-learning can learn meaningful patterns from local observations, but also reveal scalability and representation limitations in complex environments.

---

## Discussion
The results indicate that reinforcement learning can be effectively applied to Minesweeper under constrained settings. However, the reliance on tabular representations limits the agent’s ability to scale to larger boards or higher mine densities. Partial observability further increases learning complexity.

---

## Limitations
- Large state space even with abstraction
- No explicit probabilistic reasoning
- Poor scalability to complex boards
- High dependency on reward design

---

## Future Work
- Extension to Deep Q-Networks (DQN)
- Incorporation of probabilistic inference methods
- Improved state representation
- Training on larger and more complex boards
- Enhanced visual analytics within the Pygame interface

---

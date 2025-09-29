# Q-Learning Hyperparameter Experiment

This project explores how three key hyperparameters—learning rate (`alpha`), discount factor (`gamma`), and exploration rate (`epsilon`)—affect the performance of the Q-learning algorithm in a 10×10 GridWorld environment. The aim is to analyze the impact of each parameter on cumulative reward and agent behavior.

## Project Structure

### 1. Main Code (`RL_Assignment_1.ipynb`)
- **GridWorld Setup:** Defines a 10×10 grid with 20 obstacles, start and goal positions, and deterministic transitions.
- **Q-learning Implementation:** Includes the Q-learning algorithm using an ε-greedy policy and Q-value updates. Experiments are performed by varying hyperparameters.
- **Visualization:** Plots the grid layout and learning curves for each hyperparameter setting.

### 2. Figures
- **GridWorld Layout (`GridWorld Layout.png`):** Visual depiction of the environment, obstacles, start, and goal.
- **Learning Curves:**
  - `Alpha on Q-learning.png`: Shows the effect of different learning rates (`alpha`).
  - `Gamma on Q-learning.png`: Shows the effect of varying discount factors (`gamma`).
  - `Epsilon on Q-learning.png`: Shows the effect of changing exploration rates (`epsilon`).

### 3. Code Files
- **`q_learning.py` (or inline in notebook):**
  - `GridWorld` class: Simulates the grid environment.
  - `q_learning()` function: Runs Q-learning with specified hyperparameters.

## Installation & Setup

1. **Clone the Repository**
   ```
   git clone https://github.com/RaihanSubhan/Q-Learning-Hyperparameter-Experiment.git
   ```

2. **Install Dependencies**
   ```
   pip install numpy matplotlib
   ```

3. **(Optional) Install Jupyter Notebook**
   ```
   pip install notebook
   ```

## Running the Experiments

1. **Start Jupyter Notebook**
   ```
   jupyter notebook
   ```
   Open `RL_Assignment_1.ipynb` in your browser.

2. **Experiment Workflow**
   - The notebook defines `q_learning()` for running Q-learning with chosen values of `alpha`, `gamma`, and `epsilon`.
   - Use `run_experiments()` to automatically run and visualize results for each hyperparameter.

3. **Visualizations**
   - **Learning Rate (`alpha`) Effect:** Vary `alpha` with `gamma=0.9`, `epsilon=0.1`.
   - **Discount Factor (`gamma`) Effect:** Vary `gamma` with `alpha=0.1`, `epsilon=0.1`.
   - **Exploration Rate (`epsilon`) Effect:** Vary `epsilon` with `alpha=0.1`, `gamma=0.9`.
   - Each setting generates a plot comparing cumulative rewards for different values.

## Output

- **Figures:** Saved as PNG files in the project directory.
- **Data:** Cumulative rewards per episode are stored in the `returns` variable for analysis.

## Summary

By running the provided notebook, you can systematically study how Q-learning hyperparameters influence agent performance in a grid world. The generated plots and data can be used for assignments, reports, or further research.

## Example Plots

- **Learning Rate Effect:** Line graph showing cumulative rewards for various `alpha` values.
- **Discount Factor Effect:** Plot illustrating the agent’s reward with different `gamma` values.
- **Exploration Rate Effect:** Comparison of performance for multiple `epsilon` values.

These outputs align with assignment requirements and demonstrate the role of each hyperparameter in Q-learning.

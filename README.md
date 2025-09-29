# Q-Learning-Hyperparameter-Experiment
This project investigates how the learning rate alpha, discount factor gamma, and exploration rate epsilon affect the performance of Q-learning in a 10$\times$10 GridWorld. The goal is to explore the trade-offs in Q-learning performance due to these hyperparameters, using a fixed layout with 20 obstacles.
The experiments vary one hyperparameter at a time while keeping the others fixed, and performance is measured in terms of cumulative reward per episode.

File Organization
1. Main Code (RL_Assignment_1.ipynb)

This Jupyter Notebook contains:

GridWorld Setup: The 10$\times$10 environment with 20 obstacles, start and goal locations, and the deterministic movement system.

Q-learning Implementation: The Q-learning algorithm with an $\varepsilon$-greedy policy, Q-value update, and the ability to run experiments with varying hyperparameters.

Visualization: Code for plotting the obstacle layout, as well as graphs of cumulative rewards for different values of $\alpha$, $\gamma$, and $\varepsilon$.

2. Figures

GridWorld Layout (GridWorld Layout.png): The visual representation of the 10x10 grid layout with start, goal, and obstacles.

Learning Curves:

Alpha Experiment (Alpha on Q-learning.png): Plot showing the effect of varying $\alpha$ on the performance.

Gamma Experiment (Gamma on Q-learning.png): Plot showing the effect of varying $\gamma$ on the performance.

Epsilon Experiment (Epsilon on Q-learning.png): Plot showing the effect of varying $\varepsilon$ on the performance.

3. Code (q_learning.py or inline in notebook)

GridWorld Class: A Python class that simulates the grid environment.

Q-learning Implementation: The function q_learning() implements the core Q-learning algorithm and is called with different hyperparameter settings.

Setup and Installation
Clone or Download the Repository

Clone or download the project directory to your local machine.

Dependencies

This project requires Python and a few libraries to run:

numpy

matplotlib

random

You can install the necessary dependencies using pip:

pip install numpy matplotlib

Running the Code

The primary script (RL_Assignment_1.ipynb) is a Jupyter notebook. To run it, make sure you have Jupyter Notebook installed. If not, you can install it using:

pip install notebook


Then, navigate to the project folder in your terminal and run:

jupyter notebook


This will open the Jupyter interface in your web browser. You can then open RL_Assignment_1.ipynb and execute each cell in the notebook to perform the experiments.

Instructions to Run the Experiments
Running the Q-learning Algorithm

In the notebook, the function q_learning() is defined to run Q-learning with a set of hyperparameters:

alpha: Learning rate (controls how much the Q-values are updated).

gamma: Discount factor (controls how much future rewards are considered).

epsilon: Exploration rate (controls the exploration-exploitation trade-off).

After defining the GridWorld environment, the function run_experiments() runs the experiments for each hyperparameter and generates plots.

Plotting the Results

The following plots will be generated automatically:

Learning Rate Effect: Varies $\alpha$ while fixing $\gamma=0.9$ and $\varepsilon=0.1$.

Discount Factor Effect: Varies $\gamma$ while fixing $\alpha=0.1$ and $\varepsilon=0.1$.

Exploration Rate Effect: Varies $\varepsilon$ while fixing $\alpha=0.1$ and $\gamma=0.9$.

Each experiment will generate a plot comparing the cumulative rewards for different values of the respective hyperparameter.

File Output
Figures Directory:

The figure files for each of the graphs (Alpha on Q-learning.png, Gamma on Q-learning.png, Epsilon on Q-learning.png, and GridWorld Layout.png) will be saved in the project directory as PNG files.

Generated Data:

The data for each experiment will be stored in returns (the cumulative rewards per episode for each run).

Conclusion

By running the provided Jupyter notebook, the user can explore the effects of different Q-learning hyperparameters on performance in a grid world environment. The report will summarize the results and provide guidelines for selecting optimal hyperparameter values.

Example Output

Here is an example of how the plots might look:

Learning Rate Effect: A line graph showing how different values of $\alpha$ affect the cumulative reward.

Discount Factor Effect: A line graph showing the effect of different $\gamma$ values on the agent’s ability to plan long-term.

Exploration Rate Effect: A line graph comparing the performance of different $\varepsilon$ values.

These figures should match those required in the assignment, as shown in the notebook.

Project Title: Warehouse Robot Route Optimization

Description:
This project aims to optimize the route planning for warehouse robots using the Q-learning algorithm. The warehouse environment is represented as a grid with different locations denoted by letters ('A' to 'I'). The robots need to navigate from a starting location to an ending location efficiently while maximizing rewards based on the given reward matrix.

Setup:

The project utilizes Python and NumPy for implementation.
The qLearnRoute function defines the Q-learning process. It takes the starting and ending locations as input parameters.
The reward function (R) is represented as a matrix, indicating allowed movements and rewards associated with potential actions from one state to another.
Parameters such as the discount factor (gamma) and learning rate (alpha) are specified to control the learning process.
Algorithm:

Initialize the Q-matrix with zeros.
Modify the reward matrix (R_new) to incentivize reaching the ending location by assigning a high reward.
Iterate over a specified number of episodes (800 in this case) to update the Q-values using the Q-learning algorithm.
Within each episode:
Select a random starting state.
Determine allowed actions based on the modified reward matrix.
Choose the next state randomly from the allowed actions.
Update the Q-value using the temporal difference error equation.
After learning, retrieve the optimal route from the starting to the ending location using the learned Q-values.
Return the optimized route.
Usage:
To utilize the qLearnRoute function:

Call the function with the desired starting and ending locations as arguments.
The function will output the optimized route from the starting to the ending location based on the learned Q-values.

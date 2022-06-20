Aayush Dewangan (201020401)
Aryan Kaul (201020408)

Value iteration is a method of computing an optimal MDP policy and its value. This value iteration is basically a speacial case of policy iteration, as the process od policy evaluation is stopped after one step. THe value iterationsese BELLAM OPTIMAL EQUATION, we start off with some random value function and then we iterateed this using BELLAM OPTIMAL EQUATION.

# Grid World Value Iteration

This project involves creating a  5X5 grid world environmentwith 10% blockages and applying value iteration to find the optimum policy. We have attached the code for environment and agentand below is the value iteration pseudocode that was programmed and tested .

The state space of the grid world was represented using an array of length 25 (NxM). we have used some libraries such as tkinter gor GUI implmentation and numpy and random for basic mathematical implementations like performing operations on arrays and using some random policies.


In the grid world it is possible to have three different items, square, triangle and circle. The rewards for reaching circle is 1 was and the reward for colliding with trinagle is -1 so basically the rectangle with avoid colliding with the triangle block as it have negative reward. Both the circle and traingle are terminal states. Also, for each step performed by the agent a reward of -1 is received.

## Deterministic Environment
It was first decided to implement a deterministic environment as it is easier to check is the solution is correct. The three images helps to calculate the Values and Policy derived for this environment, with triangle representing blockages and cicle representing destination or end point.


## Stochastic Environment
For the stochastic environment there is a probability of 0.7 that the agents moves as intended. This means there is a probability of 0.3 a move will be randomly selected.

Then we have usewd certain functions ormethods for caluclating the number of movement the rectangular block will perform and the number of iterations and then we will be calculating the coordinate of the rectangular block with respect to origin.

The rewards points for cicle is given as 1 and the reward point for triangular is given as -1. This conculedes that the square block will neglect the triangular block holding negative reward points.

## Functioning
We have created four buttons such as "Calculate" button that calculates the policcis of each particular grid using the random function, then "Print Policy Button" that will print the allowed movement for the square block, then "Move" button that will be initiating the movement of the square block and then the block will start its movement and it will try to finf the best optimal policy to reach the destination, and at last "Clear" button that will be clearing the entire operation.



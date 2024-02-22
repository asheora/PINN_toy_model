# PINN_toy_model : PINN model for DE : u_xx = - pi^2 sin(pi x)

A Physics informed nueral network (PINN) implementation to solve the following differential equation :

$\frac{d^2 u(x)}{dx^2} + \pi^2 \sin(\pi x) = 0 $

using a Dense Neural Network architecture with :  

1 input layer consisting of 1 node (correspnding to input x) \\
2 hidden layers consisting of 50 nodes each \\
1 output layer consisting of 1 node (corresponding to output u(x)

The $\tanh$ activation function is applied on the nodes in the hidden layer. Optimizer used is ADAM.

PINN is used to learn the solution to the above mentioned differential equation for 2 cases of boundary values :    

(Case 1) $u(x=0) = u(x=1) = 0$

(Case 2) $u(x=0) = 0, u(x=1) = 1 $


Finally, the PINN solution is compared with the analytical solution.

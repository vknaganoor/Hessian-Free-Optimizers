# Second_Order_Optimisers


Newton's Method using a Hessian:
1) File Name: Linear_Regression_Newton
2) Approach: Uses the Hessian directly to estimate the step-size for the gradient descent. Involves directly inverting the hessian.
(Estimating the double differential to calculate the Hessian and inverting is computationally expensive.)


Linear Regression for Gauss-Newton's Method using a Jacobian:
1) File Name: Linear_Regression_Gauss_Newton
2) Approach: Uses the Gauss-Newton method for approximating the Hessian. Involves directly inverting [(J^T)J].

Logistic Regression for Gauss-Newton's Method using a Jacobian:
1) File Name: Logistic_Regression_Gauss_Newton
2) Approach: Uses the Gauss-Newton method for approximating the Hessian. Involves directly inverting [(J^T)J]
             Uses sqaured loss itself so that [(J^T)J] approximates the Hessian well.

Cojugate Gradient method
1) File Name: Linear_Regression_CG
2) Approach: Makes use of conjugate gradient method for solving the Ax=b , where 'A' is the Data matrix and 'b' is the column vector containing the labels

Newton Method using Conjugate Gradient
1) File Name: Linear_Regression_Newton_CG
2) Approach: Makes use of the Newton's method with conjuagate gradient to get the step size without inversing the hessian. Conjugate gradint is used to solve z = H^(-1)g

Gaussian-Newton Method using Conjugate Gradient
1) File Name: Linear_Regression_Gaussin_Newton_CG
2) Approach: Makes use of the Newton's method with conjuagate gradient to get the step size without inversing the [(J^T)J]. Conjugate gradient is used to solve z = [(J^T)J]^(-1)g

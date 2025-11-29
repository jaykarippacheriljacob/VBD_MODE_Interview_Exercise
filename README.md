Task Description
----------------

1. Implement the differential equation using the function f(t, y, parameters) as described in Algorithm 2.

2. Implement the Runge-Kutta 4 (RK4) method following Algorithm 1.

3. Declare the following variables:
   beta = 24
   delta_E = 0.6
   mu_E = 0.15
   delta_J = 0.08
   mu_J = 0.05
   alpha = 0.003
   omega = 0.5
   mu_A = 0.1
   t0 = 0
   tend = 365
   h = 0.01
   y0 = [10, 0, 0]

4. Create a vector T where each element follows the pattern t0 + h*(i-1).
   The first element must be t0 and the last element must be tend.

5. Create a wrapper function to allow the RK4 algorithm to call function f with the required parameters.

6. Create a variable to store the solution values.
   Create a for-loop that iterates from 1 to tend/h, where:

   - In the first iteration, call RK4 with function f, y0, the first element of T, and h.
   - In the second iteration, call RK4 with function f, the output from the previous iteration, the second element of T, and h.
   - Continue this pattern for all remaining iterations.

7. Create one plot containing three subplots:

   - Subplot 1: T (x-axis) vs. the first element of y and RK4 results (y-axis). Label axes: x → "T", y → "E".
   - Subplot 2: T (x-axis) vs. the second element of y and RK4 results (y-axis). Label axes: x → "T", y → "J".
   - Subplot 3: T (x-axis) vs. the third element of y and RK4 results (y-axis). Label axes: x → "T", y → "A".

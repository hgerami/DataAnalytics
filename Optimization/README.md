<h3>Optimization Models </h3>
<p>Optimization is a key component of almost all statistical learning procedures, and can provide descriptive and prescriptive analytics. Good software for solving models exists but building models requires human insight and expertise.  </p>
<h4>Elements of Optimization Models: </h4>
<ul>
  <li>Variables: <p>Decisions that the optimization solver will pick the best value for</p> </li> 
  <li>Constraints: <p>Restrictions on those decisions that we make and the values of the variables</p></li>
  <li>Objecetive Function: <p>Measure of the quality of our optimization solution (the quality of a set of values for our variables which we are trying to maximize or minimize)</p></li></ul> 
<h4>Linear and Non-Linear Optimizations: </h4>
<p>
Linear programming is a method to achieve the best outcome in a mathematical model whose requirements are represented by linear relationships whereas nonlinear programming is a process of solving an optimization problem where the constraints or the objective functions are nonlinear. 

Non-linear programming (NLP) is the process of solving an optimization problem where some of the constraints or the objective function are nonlinear

SciPy is a general-purpose package for scientific computing with Python.
PuLP is a Python linear programming API for defining problems and invoking external solvers.
</p>
  
<h3>Optimization (linear) Example in python</h3>
  <p>The Diet Optimzation: U.S. Army sought to find optimal diets for soldiers that could meet nutrition requirements while minimizing costs.  This analysis explores the nutrition and cost associated with 64 different foods to determine the optimal diet.</p>
  <p>
  <ul>
    <li> n number of foods, and m number of nutrients</li>
    <li> aij = amount of nutrient j per unit of food i</li>
    <li> mj = minimum daily intake of each nutrient j</li>
    <li> ci = cost per-unit of food i</li>
  </ul></p>
    <p> How do we fit all of this into our variables, constraints, objective function template?
  <ul>
    <li> Variables (decisions): xi = amount of food i in daily diet </li>
    <li> Constraints: US army they require that the daily intake of nutrient j is between lower and upper limit
      <ul><li>sumof(aij * xi) >= mj for each nutrient j</li><li>sumof(aij * xi) <= Mj for each nutrient j</li></ul>
      <ul><li>obvious constraint: xi >= 0  that means it is impossible to eat negative amounts of food</li></ul></li>
    <li> Objective Function: minimize sumof(ci * xi) </li>
   
  </ul></p>
  <br> <a href="US_Army_Diet_Optimization_Example.ipynb">Linear Optimization Example with Python</a>
<br>
  <b> Reference: Adopted from ISYE 6501, Introduction to Analytical Modleing Georgia Tech Courses</b><br>
<h3>Optimization (Non-linear) Example in python</h3>
  <p>In this example the allocation of a financial portofilio is optimized for any set of given stocks and time frame, That means the optimized will find how much of a portfolio’s funds should be allocated to each stock to optimize its performance. While a portfolio can be optimized for many different metrics, in this example the optimizer maximize the Sharpe Ratio. The optimizer function will return several portfolio statistics: stock allocations (allocs), cumulative return (cr), average daily return (adr), standard deviation of daily returns (sddr), and Sharpe ratio (sr). </p>

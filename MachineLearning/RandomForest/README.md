<h2> Decision Tree and Random Forest</h2>

<p> A decision tree is a supervised learning algorithm used for both classification and regression problems. Simply put, it takes the form of a tree with branches representing the potential answers to a given question. There are metrics used to train decision trees. One of them is information gain and is further explained here.
</p>
<p>
<h3>Design elements for decision tree</h3>
<ul>
<li>Which attributes to use when building a tree?</li>
<li>How to determine the split point for an attribute?</li>
<li>How many trees should the forest contain?</li>
<li>When do you stop splitting leaf nodes?</li>
</ul>
</p>
<p><h3>Entropy:</h3>
Entropy is an information theory metric that measures the impurity or uncertainty in a group of observations. It determines how a decision tree chooses to split data. The image below gives a better description of the purity of a set:
</p>
<div align="center">
<img  align="center" src="entropy_1.jpg" width="75%"  />
</div>

<h3>Example of Entropy Calculation:</h3>
<div align="center">
<img  align="center" src="entropy_calculation.jpg" width="75%"  />
</div>

<h3>Conditional Entropy:</h3>
<div align="center">
<img  align="center" src="conditional_entropy.jpg" width="75%"  />
</div>

<h3>Information Gain</h3>
<ul>
<li>
We can define information gain as a measure of how much information a feature provides about a class. Information gain helps to determine the order of attributes in the nodes of a decision tree.
</li>
<li>
We can use information gain to determine how good the splitting of nodes in a decision tree and it can help us determine the quality of splitting.</li>

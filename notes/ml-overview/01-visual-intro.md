## ML Terms
- Classification: categorizing data
- Training: creating a model
- Forks: if-then statements to define patterns in data
- Branches: the splitted data (done by forks).
- Split point: the value between the branches

## Tradeoffs
See the full metrics below ![metrics](https://github.com/rosatiara/machine-learning-for-software-engineers/blob/master/notes/ml-overview/metrics.png)

## The best (optimal) split
At the best split, the results of each branch should be as homogenous as possible.

Calculating the optimal split can be done by **gini index, cross entropy, information gain, etc.** 

Note: The notes below is from [this](https://blog.quantinsti.com/gini-index/) website. Check it out! It's a great one!

### Gini Index
#### Splitting measures
Splitting measure is a method where we decide the relevance and importance of each of the attributes.
**The most relevant will be at the root node.** and further traversing down by splitting the nodes.

The more we go down the tree, the level of impurity decreases. This leads to a better classification or best split at each node.

#### Information Gain
A method used to **determine which feature gives us the maximum information**

Information Gain is: 
- **Based on the concept of entropy** (the degree of uncertainty, impurity, or disorder)
- Aim to **reduce the level of entropy**, starting from the root node to the leave nodes.

#### So what actually Gini Index is?
Gini Index or Gini Impurity measures **the degree*** or probability **of a particular variable being wrongly classified** when it is randomly chosen.
*the degree of Gini Index varies between 0 and 1.

Pure = all the elements belong to a single class.
0 = all elements belong to **a certain class** / there exists only one class
1 = all elements are randomly distributed across 
**various classes**
0.5 = elements are **equally distributed** into some classes
##### Gini Index Formula
![gini](notes\ml-overview\gini-index.png)


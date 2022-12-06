![](https://github.com/pgmpy/pgmpy/actions/workflows/ci.yml/badge.svg?branch=dev)

# A Bayesian Approach to University Venue Allocation

## Project submitted in fulfilment of an honours degree

# How The Program Works

Program allocates courses to venues while taking into consideration the uncertainty between between features affecting venue allocation and the uncertainty of conflicting constraints.

- The baseline Bayesian Network was cosntructed from expect knowledge. 

|![Baseline model](./research%20report/images/Untitled%20Diagram.drawio%20(3).png)| 
|:--:| 
| **Baseline Bayesian Network** |

- Only synthetic data was used for this project and it was sampled from the baseline model using Bayesian Forward propagation. 
- The conditional probability tables between features(nodes)
are gernerated randomly.

|![Conditional probabbilities](./research%20report/images/download%20(1).png)| 
|:--:| 
| **Random Casual Probabilities** |

- Greedy hill climb search with random restarts was used for Structure Learning, while Bayesian Parameter Learning using a BDeu prior was used for Parameter Learning.

- Inference was performed using Variable Elimination and a MAP query was done to get venue predictions given some evidence.

- The structures were evaluated using the the log likelihood score.

# How To Run The program
- Install all required libraries by uncommenting the install libraries cell in the jupyter notebook
- After installing run all remaining cells
- To change the casual relations in the baseline network or completely change the digraph





# Course 1: Probabilistic Graphical Models 1: Representation

## Week 1

### Introduction and Overview

#### Welcome

1. Around 10-15 hours per week

#### Overview and Motivation

1. In PGM, why the word model? (Keeps data, algorithm, domain knowledge separate)
1. Why the word probabilistic? (Handles uncertainity - partial knowledge of the world, noisy observations, phenomena not covered by the model, and inherent stochasticity.)
1. Why graphical? (From the perspective of CS - uses knowledge of graphs to define complex systems. Joint distributions over random variables.)
1. What are two primary classes of PGM? (Bayesian networks and Markov networks)
1. What are Bayesian networks? (One of the two main classes of PGM which uses a directed graph for representation. Random variables are represented as nodes in the graph. The edges represent the probabilistic connections between the edges.) 
1. What are Markov networks? (The other class is known as Markov networks which uses undirected graphs.)
1. What are the advantages of using graphical model? (1. intuitive and compact data structure 2. efficient reasoning using general-purpose algorithms 3. Sparse parameterization (feasible elicitation and learning from data))

#### Distributions

1. What is a joint distribution?
1. What are parameters and independent parameters in the context of a joint probability distribution?
1. What is conditioning? What is reduction?
1. After reduction, is it still a probability distribution? (No, doesn't sum to 1) If not, how to convert it to a probability distribution? (Renormalization)
1. What is marginalization? (A procedure that takes a probability distribution over a larger set of variables and produces a probability distribution over a smaller subset of them)

#### Factors

1. What is a factor?
1. What is the scope of a factor? (the variables (not constants) in its domain)
1. How to perform a product of two factors?
1. What is factor marginalization?
1. How to marginalize a factor?
1. What to perform factor reduction?
1. Why are factors useful? (1. fundamental building blocks for defining distributions in high-dimensional spaces 2. set of basic operations for manipulating these probability distributions)

### Bayesian Network fundamentals

#### Semantics and factorization

1. What are steps in solving a problem? (1. Define a graph based on the problem at hand. 2. Define CPDs at each node)
1. What is a Bayesian network? (A DAG whose nodes represent r.v.s and for each node there is CPD defining its dependency on parents)
1. What is the chain rule formulae for BN?
1. Prove that Bayesian Network is a legal probability distribution.

#### Reasoning pattern

1. What is causal reasoning? (reasoning goes from top to bottom in the graph)
1. What is evedential reasoning? (reasoning goes from bottom to top in the graph)
1. What is intercausal reasoming? (reasoning happens in a lateral direction)
1. How does nodes that have no lateral connectons still related in an inter-causal way?

#### Flow of reasoning patterns

1. What is an active trail in a graph when nothing is observed?
1. When and how can influence flow in graph when no node is observed? Which case doesn't lead to any influence flow?
1. When one or more node/nodes is/are observed, how does the above scenario change?
1. What is an active trail in a graph when some nodes are observed?

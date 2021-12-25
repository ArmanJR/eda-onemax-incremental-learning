# Incremental Learning EDA on One-Max
Incremental Learning implementation of Estimation of Distribution Algorithm (EDA) on one-max problem

## What are EDAs?
Estimation of distribution algorithms (EDAs), sometimes called probabilistic model-building genetic algorithms (PMBGAs), are stochastic optimization methods that guide the search for the optimum by building and sampling explicit probabilistic models of promising candidate solutions. Optimization is viewed as a series of incremental updates of a probabilistic model, starting with the model encoding an uninformative prior over admissible solutions and ending with the model that generates only the global optima. (from Wikipedia)

## What is One-Max?
The OneMax Problem or BitCounting is a simple problem consisting in maximizing the number of ones of a bitstring.

## How is Incremental Learning different from simple EDAs?
In incremental learning approach, instead of generating probability vector in every iteration, we modify the last P as following:
`p[i] = p[i] + landa * (best[i] - p[i])`
Where `landa` is the learning rate (i.e. 0.02) and `best` is the fittest vector in our population.

## Executing program
You can run the [notebook on Google Colab](https://colab.research.google.com/drive/1N-zVRL0CU6Q4xYaIun7HHT2-Lt8r-Z--?usp=sharing).

## Author
- Arman Jafarnezhad

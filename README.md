# TravellingSalesmanProblem-Genetic-Algorithm

# Problem:
Given a list of cities and the distances between each pair of cities, what is the shortest possible route that visits each city and returns to the origin city?

# Genetic Algorithm:
Genetic algorithm (GA) is a search technique used to find approximate solutions to combinatorial optimization problems. The genetic algorithms are more appropriately said to be an optimization technique based on natural evolution. They include the survival of the fittest idea algorithm. The idea is to first “guess” the solutions and then combining the fittest solution to create a new generation of solutions, which should be better than the previous generation.

# Working of the Program:
•	User enters the number of cities (N)
•	Symmetric matrix of N x N is created with distances between each city being a random number.
•	User enters the number of instances in the Population (P)
•	A list of lists is created which contains P lists, each containing a random sequence of traversal.
•	Fitness Function- Calculates the sum of distances of traversal for every instance of the population.
•	Elitism Rate- User enters the Elitism rate which decides the number of instances of Population that directly go to the next generation.
•	Sort the population in ascending order based on the fitness of each instance of the population.
•	Best instances after sorting are directly appended to the next generation based on the elitism rate.
•	Using the sorted pool of Parents, consider the best 50% in the pool which will be used to create offsprings.
•	Offsprings are generated using the ordered crossover method by choosing any two random parent sequences in the first 50% of sorted pool of Parents.
•	Each pair of parents generate 2 offsprings, which ensures that the instances in the population for every generation remain almost the same (including some instances due to elitism)
•	Mutation Rate- User enters the mutation rate which decides whether swap mutation of the generated offsprings is to be done or not.
•	User also enters the number of generations that are to be created. 
•	The process repeats for each generation
•	For each generation, the minimum of the fitness function is considered and a graph is plotted which shows the decrease in the fitness as the number of generations progresses.

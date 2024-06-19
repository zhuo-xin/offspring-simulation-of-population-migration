# offspring-simulation-of-population-migration
Simulate two populations with migration each other

Task: Simulate two populations, each of which has n individual observations and m variables, where you specify the values of n and m at the start of the simulation.

Each of the variables will start with 2 possible categories, which can be labelled as 0 and 1. 

1.Start by simulating frequencies for the first category for every one of the variables, simulating separate probabilities for each of the populations so that you end up with a mx1 vector of probabilities for each population.

2.Simulate the first generation of each population: for each of n individuals and for each of the m variables, select a category based on the probabilities in that population.

3.Simulate G more generations. In each generation and in each population, “breed” that population one generation by selecting two parents from the previous generation for each child in the new population. Then generate the child by selecting one of the values its two parents have for each variable. Each parent may be the parent of more than one child in the next generation. Repeat this process using the n children in one generation as the set of n possible parents of the next generation.

4.Modify the simulation so that there are two sexes of individuals, M and F. When breeding the population, each child must have one M parent and one F parent. The child will be M or F randomly with 50% probability for each.

5.Modify the simulation further so that the two populations have some migration between them. In other words, at each generation a specified proportion M of the parents will be selected from the other population instead of this population (so when breeding pop 1, M*2*n of the parents will be from pop 1 and (1-M)*2*n of the parents will be from pop 2, and similarly in reverse for breeding pop 2).

The output of the code can be a dataset which contains the final generation of the two populations

# NSGA-II for cooperative combat model of ground-based multi-platform  
This is the priliminary work of my graduate project.  
a bi-objective multi-stage sensor-weapon target assignment model under uncertainty is established  
NSGA-II algorithm is used to solve this problem. this work is modified based on the work of Aravind Seshadri  
url: https://www.mathworks.com/matlabcentral/fileexchange/10429-nsga-ii-a-multi-objective-optimization-algorithm  

////File name - Its function  
NSGA2_on_DSWTA - main function  
Generator - generate basic parametors of the model to verifying the proposed algorithm.  
initialize_the_population - generate the initial population of NSGA-II  
evaluate_objective - calculate the two objective value of the population  
non_dominated_sorting - use the fast non-dominated sorting algorithm to sorting the population as well as calculating its crowded distance  
tournament_selection - use the tournament selection mechanism to select a subset of population based on its rank untill fullfilling the pool  
genetic_operator - use the designed crossover and mutation operator to generate new offspring.  
repair_operator - repair the offspring generated by genetic_operator to make it feasible under constraint.  
replace_chromosome - select individuals from hybrid population to the next generation  

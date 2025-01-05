# Evolutionary-algorithm-ES-μ+λ
This project implements an evolutionary algorithm (EA) with a (mu + lambda) strategy for optimizing a two-dimensional function. The algorithm can be used for both minimization and maximization of the objective function.

# Objective Function
The algorithm can optimize any two-dimensional function 𝑓(𝑥,𝑦). By default, the following function is used:

f(x, y) = (9 * x * y) / exp(x ** 2 + 0.5 * x + y ** 2)

![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/88f5505d-1906-44fb-bccf-1b0d34b7b9b4)

However, you can define your own function in the code file.

# Algorithm Parameters

- 𝜇  Size of the parent population (default is 128).
- 𝜆  Size of the offspring population (default is 512).
- 𝜎  Standard deviation of the mutation (default is 0.1).
- ITERATIONS Number of algorithm iterations (default is 200).

  # Evolutionary Strategy

Selection: Tournament selection is used, where a certain number of individuals are randomly selected for a tournament, and then the best one is chosen as a parent.

Crossover: Averages-based crossover in the extended variant is applied, which combines features of two parents in proportion determined by a random value 𝑎 from the interval [0,1]

Mutation: Gaussian mutation is utilized, which introduces random changes in individual features by adding Gaussian noise.

Elimination: The best individuals from the offspring population are selected for the next iteration, while the worst ones are removed from the parent population.

# Example Results
WolframAlpha Results:

![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/e088129d-1474-4981-9f84-4cb6c77722bc)

![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/bd8dd48b-5c0c-480f-bf96-ca4b15608339)

Based on the analysis of the plots of the function below, it can be observed that the function has two minima and two maxima.

The minima of the function are located in the second and fourth quadrants of the coordinate system. They are as follows:
1) Minimum of f(x,y) ≈ -2.43687 for (x,y) ≈ (-0.84307, 0.707107)
2) Minimum of f(x,y) ≈ -1.19715 for (x,y) ≈ (0.59307, -0.707107)

The maxima of the function are located in the first and third quadrants of the coordinate system. They are as follows:
1) Maximum of f(x,y) ≈ 1.19715 for (x,y) ≈ (0.59307, 0.707107)
2) Maximum of f(x,y) ≈ 2.43687 for (x,y) ≈ (-0.84307, -0.707107)
   
Find Minimum using Evolutionary-algorithm-ES-μ+λ

![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/0b66b149-b532-4841-b551-c99ff48747e7)
![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/2ce99211-bab6-4071-af04-e9a3ea760e61)
![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/349be6c4-1c82-4964-997c-71be9aeaa1a3)
![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/8f4046b6-e79b-4664-a391-eb185ad46762)


Find Maximum using Evolutionary-algorithm-ES-μ+λ

![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/bba9d311-8fb6-45a0-944d-60bd97331dfb)
![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/6fe986f1-050c-4371-a372-238c217a9edd)
![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/9368e69f-8f5c-4c53-8901-922fcb484f2b)
![image](https://github.com/mik00laj/Evolutionary-algorithm-ES-mu-lambda/assets/108618874/6daeb06b-f8b7-4121-a580-8444d5a2151a)




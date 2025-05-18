# 🧬 Genetic Algorithm (GA)

Genetic Algorithm (GA) is a **metaheuristic optimization algorithm** inspired by the process of **natural selection** and **genetics**. It is commonly used for **solving complex optimization** and **search problems** where traditional methods may not perform well.

---

## 📌 Key Concepts of Genetic Algorithm

### 1. **Population**
A set of possible solutions (called individuals or chromosomes). Each individual represents one possible solution to the problem.

### 2. **Chromosome (Individual)**
A candidate solution, often represented as a string, list, or array. For example, in a TSP, a chromosome could be a permutation of cities.

### 3. **Gene**
A part of the chromosome that holds specific information. For example, a city in a route.

### 4. **Fitness Function**
Evaluates how "good" or "fit" an individual solution is. Higher fitness means a better solution.

### 5. **Selection**
The process of choosing the best individuals from the population to pass their genes to the next generation.

### 6. **Crossover (Recombination)**
Combines two parent solutions to produce one or more offspring. It mimics biological reproduction.

### 7. **Mutation**
Applies random changes to an individual’s genes to maintain genetic diversity and explore new parts of the search space.

### 8. **Termination Condition**
The algorithm stops when it reaches a predefined number of generations or when the fitness no longer improves.

---

## 🔁 Genetic Algorithm Workflow


1. Initialize a random population
2. Evaluate the fitness of each individual
3. Select the fittest individuals for reproduction
4. Perform crossover to produce offspring
5. Apply mutation to offspring
6. Form a new population and repeat from step 2
7. Stop when termination condition is met


## 🧠 Analogy with Natural Evolution

| GA Term       | Natural Analogy        |
|---------------|------------------------|
| Population    | Group of organisms     |
| Chromosome    | DNA                    |
| Gene          | A trait                |
| Fitness       | Survival chance        |
| Selection     | Natural selection      |
| Crossover     | Sexual reproduction    |
| Mutation      | Genetic mutation       |

---

## 🛠️ Applications of Genetic Algorithms

- 🧭 **Travelling Salesman Problem (TSP)**
- 📈 **Feature selection in Machine Learning**
- 🤖 **Robot path planning**
- 🧠 **Neural network architecture optimization**
- 🧬 **Bioinformatics** (e.g., gene sequencing)
- 📦 **Inventory and logistics optimization**

---

## ✅ Advantages

- Works well for **complex search spaces**
- Can handle **non-linear** and **discrete** problems
- Does **not require gradient** information
- Provides **near-optimal solutions** quickly

---

## ❌ Disadvantages

- No guarantee of finding the **global optimum**
- Requires careful **tuning of parameters** (mutation rate, crossover rate, etc.)
- Can be **computationally expensive**
- May **converge prematurely** if diversity is lost

---

## 🔧 GA Parameters to Tune

| Parameter         | Description                                      |
|------------------|--------------------------------------------------|
| Population Size   | Number of individuals in each generation         |
| Mutation Rate     | Probability of random mutation                   |
| Crossover Rate    | Probability of crossover                         |
| Generations       | Number of iterations the GA will run             |
| Selection Method  | Tournament, Roulette Wheel, Rank-based, etc.     |

---

## 📚 Summary

Genetic Algorithms are a **powerful tool** for solving optimization problems by simulating the process of **evolution**. With concepts like **selection**, **crossover**, and **mutation**, they explore the solution space effectively and are widely used across industries and research fields.


# 🧬 Example of Travelling Salesman Problem using Genetic Algorithm (TSP-GA)

A Python-based implementation of the **Genetic Algorithm (GA)** to solve the **Travelling Salesman Problem (TSP)** — one of the most famous combinatorial optimization problems.

---

## 📌 Problem Statement

Given a set of cities and the distances between every pair of cities, the task is to find the shortest possible route that visits each city exactly once and returns to the origin city.

---

## 🚀 How It Works

This project uses the core concepts of **Genetic Algorithms**, such as:

- **Population Initialization** (random routes)
- **Fitness Evaluation** (based on total travel distance)
- **Selection** (fitness-proportionate)
- **Crossover** (Ordered Crossover - OX)
- **Mutation** (Swap Mutation)

The algorithm iteratively improves the population of solutions to reach an optimized (shortest) path.

---

## 🧠 Genetic Algorithm Flow

```text
1. Initialize a population of random routes
2. Evaluate fitness (shorter routes = higher fitness)
3. Select the fittest parents
4. Perform crossover to produce offspring
5. Apply mutation to introduce variation
6. Repeat for a set number of generations or until convergence
```
## Sample Output 
```bash
Initial Best Distance: 17.82
Gen 0: Best Distance: 17.82
Gen 10: Best Distance: 15.23
Gen 20: Best Distance: 13.47
...
Final Best Route: ['B', 'C', 'D', 'E', 'A']
Final Best Distance: 12.81
```
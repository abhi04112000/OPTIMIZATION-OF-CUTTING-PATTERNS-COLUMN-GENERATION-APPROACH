# Optimization of Cutting Patterns | Column Generation Approach

## Project Overview

This project focuses on optimizing cutting patterns to minimize material wastage and maximize material usage for a given stock length. The problem is approached using a Column Generation technique, which involves decomposing the problem into a master problem and a subproblem, and utilizing CPLEX to generate dual values and optimize cutting patterns.

## Table of Contents

- [Project Description](#project-description)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Model and Techniques](#model-and-techniques)
- [Results](#results)
- [Usage](#usage)
- [License](#license)
- [Contributing](#contributing)

## Project Description

The project aims to reduce material wastage by selecting optimal cutting patterns and maximizing the usage of a given stock length. The approach uses Column Generation, a technique that iteratively solves a linear programming (LP) master problem and an integer programming (IP) subproblem until optimality is achieved. The performance of the Column Generation approach is compared with the Knapsack method.

## Features

- **Optimal Cutting Patterns:** Reduced material wastage by selecting the most efficient cutting patterns.
- **Column Generation Technique:** Decomposed the problem into a master LP problem and a subproblem IP for efficient pattern generation.
- **Performance Comparison:** Compared solution times and effectiveness with the Knapsack method.
- **Minimal Waste:** Achieved only 0.88% material waste with the Column Generation approach.

## Technologies Used

- Python
- CPLEX Optimization Studio
- Linear Programming (LP)
- Integer Programming (IP)
- Column Generation Technique

## Model and Techniques

### Column Generation Approach

- **Problem Decomposition:** Decomposed the cutting pattern problem into a master problem (LP) and a subproblem (IP).
- **Iterative Optimization:** Repeatedly solved the master and subproblem until the reduced cost (Zj - Cj) became negative, indicating optimality.
- **CPLEX Utilization:** Used CPLEX software to generate dual values and solve the LP and IP problems.

### Performance Comparison

- **Knapsack Method Comparison:** Compared the Column Generation approach with the Knapsack method in terms of solution time and efficiency.
- **Material Waste:** Achieved only 0.88% waste with the Column Generation approach, significantly less than the Knapsack method.

## Results

- **Material Waste:** Achieved a minimal material waste of 0.88% with the Column Generation approach.
- **Efficiency:** The Column Generation approach required significantly less time compared to the Knapsack method.

## Usage

1. **Data Preparation:** Prepare input data for stock lengths and cutting patterns in the required format.
2. **Configuration:** Adjust model parameters and settings in the project files.
3. **Run Optimization:** Execute the optimization script using CPLEX to generate optimal cutting patterns and evaluate performance.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Feel free to contribute to this project by opening issues or submitting pull requests. For more details, see the [CONTRIBUTING](CONTRIBUTING.md) guidelines.

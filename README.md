# Boolean Networks and GRNs Reconstruction

## Repository Name

`boolean-networks-grn-reconstruction`

## Description

Python tools for Boolean Network simulation, outlier detection using GESD, and analysis of periodic orbits. Includes methods for outlier detection, Boolean network state enumeration, and determination of attractors and basins of attraction.

## Exercise 1: Outlier Detection Algorithm

### (a) Implementing GESD Test

- Implement the `GESD_test()` method in `exercise_1.py` to perform outlier detection.
- The method should execute the Generalized Extreme Studentized Deviate (GESD) test as described in Lecture V10, page 36, or the provided link.
- Use `scipy.stats.t.ppf()` for calculating the percentage point with one tail probability.

### (b) Testing GESD

- In `exercise_1.py`, generate two normally distributed datasets (size 10 and 40) with 0 mean and unit variance.
- Introduce random outliers and apply `GESD_test()` to detect them.
- Report the critical values, deviation statistics, and iteration where outliers are detected.

### (c) Analysis

- Evaluate if GESD detected all outliers in the datasets.
- Discuss the effectiveness of the GESD algorithm and potential reasons for any failures.

## Exercise 2: Boolean Network Simulation

### (a) Simulating the Boolean Network

- Write a program in `exercise_2.py` to simulate the Boolean Network.
- Convert binary levels of genes to integers where A is the least significant bit and F is the most significant.
  
  **Questions:**
  
  1. How many initial states are possible for this gene network?
  2. When does it make sense to stop the propagation and why?
  3. Which sequences of states (trajectories) are observed starting from states 0, 1, 6, 15, 37, or 52?

### (b) Periodic Orbits

- Determine attractors and basins of attraction by tracking all possible initial states and their returns to previously visited states.

  **Questions:**
  
  1. List the orbits with their lengths and basins of attraction.
  2. Provide the relative coverages of the state space by the basins of attraction.

## Usage

1. Implement the methods as described in the respective sections of `exercise_1.py` and `exercise_2.py`.
2. Run the scripts to test outlier detection and Boolean network simulation.
3. Report results and analyze as specified.

## Requirements

- Python 3.x
- scipy
- numpy

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

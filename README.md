# Quantum vs Classical Randomness Analysis

## Project Overview

Random number generation is fundamental to cryptography, simulations, and machine learning. Classical computers typically use pseudo-random number generators (PRNGs), which are deterministic algorithms. Quantum computing, however, can produce randomness through quantum superposition.

This project performs a comparative statistical analysis between classical and quantum random number generators using Python and Qiskit.


## Objectives

* Generate random bits using a classical method
* Generate random bits using a quantum circuit
* Compare statistical properties of both sources
* Measure entropy and distribution balance
* Perform chi-square goodness-of-fit testing
* Visualize and interpret randomness quality

## Methodology

### Classical RNG

* Uses Python's built-in `random` module
* Produces pseudo-random bits
* Fast but algorithmically deterministic

### Quantum RNG

* Built using Qiskit
* Uses a Hadamard gate to create superposition
* Measurement collapses the qubit into 0 or 1
* Simulated using QASM simulator

### Statistical Analysis

The following metrics are computed:

* Frequency of 0s and 1s
* Mean and variance
* Shannon entropy
* Chi-square goodness-of-fit test
* Bar chart visualization

## Tech Stack

* Python
* Qiskit
* NumPy
* SciPy
* Matplotlib
* Jupyter Notebook


## Sample Results (Expected)

In an ideal random process:

* Probability(0) ≈ 0.5
* Probability(1) ≈ 0.5
* Entropy ≈ 1
* Chi-square p-value should not indicate strong bias

Both classical and quantum generators should appear close to uniform, though classical RNG is fundamentally pseudo-random.

## Key Insights

* Quantum superposition can be used to generate random bits
* Classical RNGs are deterministic but statistically strong
* Entropy is a useful metric for randomness quality
* Simulator-based quantum randomness behaves close to ideal randomness

## Limitations

* Quantum results are obtained from a simulator, not real hardware
* Only single-qubit randomness is tested
* Limited statistical tests applied
* Performance depends on simulator backend

## Future Improvements

* Test on real quantum hardware
* Add runs test and autocorrelation analysis
* Compare multiple PRNG algorithms
* Study randomness under quantum noise
* Perform large-scale statistical batteries

## Author

**Shivani Hebbar**
MSc Data Science

## Acknowledgment

Built as a beginner-friendly exploration of quantum randomness using Qiskit and statistical analysis.

# Quantum_Computing_Tasks

# Quantum Computing Tasks

This repository contains the solutions and explanations for a series of quantum computing tasks implemented using Qiskit.

## Overview

This collection of tasks explores fundamental concepts in quantum computing, including superposition, entanglement, and basic quantum game simulations. Each task is implemented within a Jupyter Notebook.

## Task Breakdown

### Task 1: Forced Superposition

* **Goal:** Create a 2-qubit circuit where Qubit 0 is in the $|+\rangle$ state, Qubit 1 is in the $|1\rangle$ state, and they are entangled such that measuring Qubit 0 always gives the opposite result of Qubit 1.
* **Implementation:** The implementation for this task can be found in the `Task1_Forced_Superposition.ipynb` notebook.
* **Verification:** The circuit is simulated for 1000 shots, and the measurement counts are plotted to verify the opposite correlation.

### Task 2: Entanglement Witness

* **Goal:** Build a circuit to demonstrate how modifying one qubit of an entangled pair can break the entanglement.
* **Implementation:** The implementation for this task can be found in the `Task2_Entanglement_Witness.ipynb` notebook.
* **Analysis:** The measurement outcomes are analyzed to see if they remain random (50/50), which would indicate that the entanglement is still present. A deviation from this suggests that the entanglement has been affected by the error.

### Task 3: Opposite-Measurement Entanglement

* **Goal:** Create a circuit where two qubits are entangled such that measuring one always gives the opposite result of the other (if Qubit 0 is 0, Qubit 1 is 1, and vice versa).
* **Implementation:** The implementation for this task can be found in the `Task3_Opposite_Measurement.ipynb` notebook.
* **Verification:** The circuit is simulated for 1000 shots, and the resulting histogram should ideally show only '01' and '10' outcomes.

### Task 4: Quantum Coin Flip Game

* **Goal:** Simulate a quantum coin flip game between Alice and Bob. Alice prepares a qubit in the $|+\rangle$ state, and Bob randomly measures it in either the X or Z basis.
* **Winning Conditions:** Bob wins if he measures $|+\rangle$ or $|0\rangle$; Alice wins otherwise.
* **Implementation:** The implementation for the non-entangled version of the game can be found in `Task4_Quantum_Coin_Flip_Non_Entangled.ipynb`, and the entangled version in `Task4_Quantum_Coin_Flip_Entangled.ipynb`.
* **Analysis:** The win rates for both scenarios are calculated and compared.

### Essay Question

* **Content:** An explanation of how entanglement and superposition enable quantum speedups, drawing examples from the tasks. It also discusses why classical systems cannot replicate this behavior.
* **Location:** The essay can be found in `Essay_Questions.ipynb` or a dedicated section within the `QC Task.ipynb` notebook.

## How to Use

Each task's implementation is contained within a Jupyter Notebook (`.ipynb` file). To run the code, ensure you have Qiskit and its necessary components installed:

```bash
pip install qiskit qiskit-aer random

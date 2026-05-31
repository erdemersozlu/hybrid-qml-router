# Hybrid QML Router Agent 🧠⚛️

This project is a rule-based AI agent that autonomously analyzes the complexity and features of a given dataset to determine whether it should be routed to a **Classical Machine Learning** model (via Scikit-learn) or a **Quantum Machine Learning** model (via Qiskit). 

## 🎯 Project Objective
The main motivation behind this project is to bridge classical and quantum computing paradigms. Instead of isolating them, this system dynamically leverages the most efficient approach based on the specific workload and data dimensions. 

The architecture is strictly built using **Object-Oriented Programming (OOP)** principles—such as modular classes, inheritance, and encapsulation—to ensure the codebase remains scalable and maintainable.

## 🏗️ Architecture & Workflow
1. **Data Profiler:** Analyzes the dataset's dimensions, feature counts, and data types.
2. **Router Agent:** Executes the decision-making mechanism based on predefined thresholds.
    * *Low-dimensional, complex data* -> Routes to `QuantumSolver` (Encodes data into a quantum circuit using Angle Encoding).
    * *High-dimensional, linear data* -> Routes to `ClassicalSolver` (Processes data using traditional SVM/Random Forest models).
3. **Execution:** Runs the selected solver and logs the results and decision rationale.

## 🚀 Installation

To run this project locally, follow these steps:

```bash
git clone https://github.com/erdemersozlu/hybrid-qml-router
cd hybrid-qml-router
pip install -r requirements.txt
python main.py
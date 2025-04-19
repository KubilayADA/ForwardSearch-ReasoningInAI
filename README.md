**GitHub Repository**
https://github.com/KubilayADA/ForwardSearch-ReasoningInAI

# 🔍 Project Overview - Forward Search - Bonus Task for SE_14 Assessment 

A Python project implementing **Forward Search** and **Model Checking** algorithms for reasoning in propositional logic. The project is designed to evaluate logical sentences and check whether a query can be proven true or false based on a knowledge base of logical formulas.

This project is part of the **SE_14 Artificial Intelligence Basics** assessment at CODE University. The task involves implementing and comparing two algorithms—**Forward Search** and **Model Checking**—for solving propositional logic problems. The goal of the project is to demonstrate how both algorithms work on different logical problems, compare their results and performance, and learn to handle logical reasoning in the context of AI.
---

## 📁 Repository Structure

```bash
Forward Search - Homework/
├── logic/                     # Contains logic-related classes 
│   ├── biconditional.py       # Biconditional logic implementation
│   ├── conjunction.py         # Conjunction (AND) logic implementation
│   ├── disjunction.py         # Disjunction (OR) logic implementation
│   ├── implication.py         # Implication logic implementation
│   ├── negation.py            # Negation logic implementation
│   ├── sentence.py            # Base class for all logical sentences
│   ├── symbol.py              # Symbol class for propositional logic
├── solvers/                   # Contains reasoning algorithms
│   ├── forward_search.py      # Forward search algorithm implementation
│   ├── model_check.py         # Model checking algorithm implementation
├── main.py                    # Main script to test and compare algorithms
├── README.md                  # Documentation for the project
```

**Explanation of the Project Structure:**
- The `logic/` directory contains the logic classes that represent propositional logical expressions.
- The `solvers/` directory contains the solvers that implementing the reasoining algorithms.
    **forward_search.py:** Implements the forward search algorithm, which uses a knowledge base to infer new facts until a query is proven or disproven.
    **model_check.py:** Implements the model checking algorithm,  which checks all possible models to evaluate the truth of a given query.
- The `main.py` script that ties eveything together and runs tests for both Forward Search and Model Checking algorithms on predefined logic problems. 

## How to Start the System 

**1. Prerequisites**

Please ensure you have Python 3.x installed on your system.

> No external dependencies are needed. The project use only standard Python libraries.

**2. Installation**
Clone the repository:
If you havent cloned the repository yet, you can do so by running following command:
```bash
git clone https://github.com/KubilayADA/ForwardSearch-ReasoningInAI.git
cd forward_search-reasoning-in-ai
```
**3. Running the Program**

To run the program, execute the main.py script. It will run both Forward Search and Model Checking algorithms on a series of predefined problems:
```bash
python3 main.py
```
This will trigger the testing process and display the results for each problem.

## Expected Output
- For each problem, the program will display:
The result of the model_check and forward_search algorithms.
The execution time for both algorithms in nanoseconds.

 **Example Output (Problem 1)**
 ```bash
 Testing Problem 1
... running model checking
... running forward search
... done. 

- result - model checking:  True
- result - forward search:  True
- time for model checking: 127000 ns
- time for forward search: 192000 ns
```

## Explanation of the Algorithms
**Model  Checking:**
- Definition: Works by systematically checking all possible logical models (truth assignments).
- Goal: Determine whether a specific query is logically entailed by the knowledge base.

**Forward Search:**
- Definition:Starts with a knowledge base and attempts to infer new facts.
- Goal: Derive new information using inference rules until the query is proven or disproven.



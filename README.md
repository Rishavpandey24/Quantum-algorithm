# Quantum Algorithms with Qiskit ⚛️

This repository demonstrates some of the most fundamental algorithms in quantum computing using [Qiskit](https://qiskit.org/). The implementations included here are the **Deutsch–Jozsa algorithm**, the **Bernstein–Vazirani algorithm**, **Grover’s search algorithm**, and **Shor’s factoring algorithm**. Each notebook provides both a conceptual overview and a hands-on implementation, making it easier to understand how these algorithms exploit quantum principles such as superposition, interference, and entanglement to outperform their classical counterparts.

The **Deutsch–Jozsa algorithm** is one of the earliest examples that shows a clear quantum advantage. It determines whether a given function is constant or balanced, something that would require an exponential number of queries classically but can be solved with a single query on a quantum computer. Similarly, the **Bernstein–Vazirani algorithm** efficiently finds a hidden binary string that defines a function. While the classical solution requires multiple queries, the quantum algorithm reveals the hidden string with just one execution, showcasing the power of quantum parallelism.

Another important algorithm included in this repository is **Grover’s algorithm**, which provides a quadratic speed-up for searching an unstructured database. Instead of requiring `N` queries to find a marked item in a database of size `N`, Grover’s approach finds the solution in about `√N` steps, making it one of the most practical quantum algorithms for real-world search problems. Finally, the **Shor’s algorithm** is implemented to demonstrate quantum factoring. This algorithm can factor large integers in polynomial time, a task believed to be exponentially hard for classical computers. The implications of Shor’s algorithm extend to cryptography, as it threatens the security of widely used systems like RSA.

To set up this repository, begin by cloning it from GitHub using `git clone` and then moving into the project directory. It is recommended to create a Python virtual environment with `python -m venv qenv` to keep the dependencies isolated; once created, you can activate it using `qenv\Scripts\activate` on Windows or `source qenv/bin/activate` on macOS and Linux. With the environment ready, install the required packages by running `pip install qiskit matplotlib notebook`. Qiskit provides the quantum circuit framework, Matplotlib is used for visualization, and Jupyter allows you to open and execute the provided notebooks. After installation, launch Jupyter Notebook with `jupyter notebook`, open any of the algorithm notebooks—such as `deutsch_jozsa.ipynb`, `bernstein_vazirani.ipynb`, `grover.ipynb`, or `shor.ipynb`—and you will be ready to explore the quantum algorithms interactively.

This project makes use of Qiskit for circuit construction, simulation, and visualization. All results are generated either on local simulators or using IBM Quantum cloud backends. By exploring the notebooks, you will gain hands-on experience in quantum circuit design and observe how theoretical quantum speedups translate into practical code execution.

---

## References

- Nielsen & Chuang, *Quantum Computation and Quantum Information*  
- [Qiskit Textbook](https://qiskit.org/textbook/)  
- Grover, L. K. (1996). *A fast quantum mechanical algorithm for database search*.  
- Shor, P. W. (1997). *Polynomial-time algorithms for prime factorization and discrete logarithms on a quantum computer*.  

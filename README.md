# Grovers-Algorithms
This repository contains 2, 3, and 4 qubit versions of [Grover's Algorithm.](https://en.wikipedia.org/wiki/Grover%27s_algorithm)

## What is Grover's Algorithm?
Grover's Search is a Quantum Search algorithm that can find an element in a list in only `O(sqrt(n))` time. 

This is a **huge** improvement over classical algorithms, that can only do that in `O(n)`.

## That's exciting, how do I run it?
Running this is very easy.
- Clone/Download this repo.
- Head over to [IBM's Quantum Lab.](https://quantum-computing.ibm.com/jupyter) (You might need to create an account)
- Click "Import".
- Choose one of the files included in this repo.
- Run the python code as you'd run any normal Jupyter notebook.
- To search for a specific state (for 4 qubits, say `1010`, modify the `state_to_search` variable in the code, and re-run). Note that qiskit shows the results in reverse order (MSB to LSB, so for `1010` you'll see `0101` as the result)

## Okay, but I want to create an array and find an element in it.
That's... not how it works. Quantum Computing right now is in it's infancy and so we are only dealing with bits. This algorithm is literally written with quantum registers and quantum gates (the Python code is just a wrapper for Quantum Assembly code). - Unfortunately we probably need years and years of software engineering to have a good enough abstraction to enable array creation. Maybe check back in a few years!

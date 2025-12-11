# Hilbert R-Tree

![Language](https://img.shields.io/badge/language-C-00599C.svg)

## Project Description

This project provides a C implementation of the **Hilbert R-Tree**, an advanced spatial access method. It combines the dynamic hierarchy of R-trees with the **Hilbert Space-Filling Curve** to order multidimensional geometric data.

By using the Hilbert value to organize nodes, this data structure achieves superior **spatial locality** compared to traditional R-trees. This results in better performance for packing data and executing range queries, as spatially close objects are stored closer together in the index.

### Key Features
* **Spatial Indexing:** Efficiently stores and queries multi-dimensional geometric data.
* **Hilbert Ordering:** Uses Hilbert curve values to linearize spatial objects, optimizing the structure of the tree.
* **Dynamic Operations:** Supports insertion and node splitting logic specific to Hilbert R-trees.
* **Visualization/Reference:** Includes a PDF resource explaining the underlying concepts.

---

## Project Structure

* **`hilbert_R_Tree.c`**: The core source file containing the implementation of the Hilbert R-Tree logic, node management, and testing interface.
* **`hilbert R Tree.pdf`**: Documentation/Reference material explaining the theory and algorithm used in this implementation.
* **`README.md`**: Project documentation.

---

## Technologies Used

* **Language:** C (Standard C99 or later recommended)
* **Compiler:** GCC (GNU Compiler Collection)

---

## Getting Started

### Prerequisites

Ensure you have a C compiler installed:
* **GCC** (standard on most Linux/Mac systems).

### Installation

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/YuvrajDoshi01/Hilbert-R-Tree.git
    cd Hilbert-R-Tree
    ```

---

## Compilation & Build Instructions

Since this is a single-file C implementation, you can compile it directly using `gcc`.

**Compile the source code:**
```bash
gcc -w hilbert_R_Tree.c -o hilbert_tree -lm
```

* **`-w`**: Suppresses compiler warnings (useful for older C style code).
* **`-o hilbert_tree`**: Names the output executable `hilbert_tree`.
* **`-lm`**: Links the math library (often required for geometric calculations).

---

## Usage

Once compiled, run the executable from the terminal:

```bash
./hilbert_tree
```

**Interactive Mode:**
The program may prompt you to enter the name of a data file or provide input values directly depending on the logic in `main()`. Ensure your input data matches the expected format.

---

## References

* **Original Paper:** [Hilbert R-Tree: An Improved R-Tree Using Fractals](https://www.cs.cmu.edu/~christos/PUBLICATIONS.OLDER/vldb94.pdf) (Kamel & Faloutsos, VLDB 1994).
* See the included **`hilbert R Tree.pdf`** for specific implementation details relevant to this codebase.


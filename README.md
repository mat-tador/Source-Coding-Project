# Information-Theory-Project

This repository contains a collection of Jupyter Notebooks and Python scripts dedicated to the implementation and analysis of fundamental **Source Coding** algorithms. The project explores lossless data compression techniques, providing practical implementations and test cases on various data types (including literary texts and DNA sequences).

## 📂 Project Structure

The project is organized into the following modules and notebooks:

### 1. `Introduction.ipynb`
An introductory notebook that sets up the working environment.
- **Libraries:** Introduction to `itertools`, `collections`, `matplotlib`, `networkx`.
- **Concepts:** Explanation of advanced Python concepts used throughout the project (List/Dict Comprehensions).
- **Data Structures:** Introduction to tree structures used in coding algorithms.

### 2. `Huffman.ipynb`
Implementation of **Huffman Coding**.
- Construction of the Huffman Tree.
- Symbol code generation.
- Compression performance analysis and visualization using `networkx`.

### 3. `Arithmetic.ipynb`
Implementation of **Arithmetic Coding**.
- Development of an *Arithmetic Encoder* and *Decoder*.
- Handling of probability intervals and precision.
- **Real-world Use Cases:**
  - Compression of the book *"War and Peace"*.
  - Compression of DNA sequences.

### 4. `SourceCoding.py`
A Python helper module containing core classes and functions used by the notebooks. It includes:
- Probability calculation functions (`gen_dict`).
- Interval management logic and binary conversions (`x_pos`, `conv_bit`).
- **Arithmetic Decoder Class:** Handles `feasible_range`, updates, and the decoding loop.
- Implementations related to Shannon coding and length calculations.

## 🛠️ Requirements & Installation

The code is written in **Python 3**. To run the notebooks, ensure you have the following libraries installed.

You can install them via pip:

```bash
pip install matplotlib networkx pillow jupyterlab
```
## 🚀 Usage

Clone the repository or download the files.

Start Jupyter Notebook or Jupyter Lab:
``` bash
    jupyter lab
```

Open and run the notebooks in the recommended order:

Introduction.ipynb (for setup and basic concepts).

Huffman.ipynb or Arithmetic.ipynb (depending on the algorithm of interest).

Important: The SourceCoding.py file must be located in the same directory as the notebooks to allow proper importing of functions and classes.
## 📊 Algorithm Features

Huffman Coding: Optimal for symbol-by-symbol coding based on integer frequencies. Includes graphical visualization of trees.

Arithmetic Coding: More efficient than Huffman for probabilities that are not powers of two. It encodes the entire message as a single number within an interval [0, 1). It handles finite precision through interval rescaling/trimming.

👤 Author

Project developed for the analysis of Information Theory class. Mattia Fiore
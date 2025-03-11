Here's an enhanced `README.md` for the [6-degrees-of-wikipedia](https://github.com/rohitpugazh/6-degrees-of-wikipedia) repository:

```markdown
# 6 Degrees of Wikipedia

## Overview

This project explores the concept of "Six Degrees of Separation" within the vast network of Wikipedia articles. Inspired by the Wikispeedia game, which challenges players to navigate between two Wikipedia articles using the shortest chain of links, this project analyzes the connectivity of Wikipedia through graph-based models. By constructing a directed graph where nodes represent articles and edges represent hyperlinks, we aim to:

- **Find the Shortest Path**: Determine the minimum number of clicks required to navigate from one article to another.
- **Approximate the Longest Shortest Path**: Identify the longest distance between any two articles in terms of link navigation.

## Features

- **Graph Construction**: Parse and decode Wikipedia datasets to build a directed graph of articles and their hyperlinks.
- **Optimization Models**: Implement various models to analyze the graph, including:
  - Direct application of the Gurobi solver for shortest path problems.
  - Random sampling to identify the longest shortest path.
  - Landmark-based approximation as an alternative analytical approach.
- **Interactive Notebook**: Utilize Jupyter Notebook (`wikispeedia.ipynb`) for interactive analysis and visualization.

## Installation & Setup

### Prerequisites

- **Python 3.7+**: Ensure you have Python installed. You can download it from the [official website](https://www.python.org/).
- **Gurobi Optimizer**: This project utilizes the Gurobi solver. Obtain a license and installation details from the [Gurobi website](https://www.gurobi.com/).

### Steps to Set Up the Project

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/rohitpugazh/6-degrees-of-wikipedia.git
   cd 6-degrees-of-wikipedia
   ```

2. **Set Up a Virtual Environment** (Optional but recommended):

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows: env\Scripts\activate
   ```

3. **Install Required Packages**:

   ```bash
   pip install -r requirements.txt
   ```

4. **Install Gurobi**:

   Follow the instructions provided by Gurobi to install the optimizer and obtain a license. Ensure that the Gurobi Python interface is correctly set up.

5. **Launch Jupyter Notebook**:

   Open the Jupyter Notebook to interact with the analysis:

   ```bash
   jupyter notebook wikispeedia.ipynb
   ```

## Usage

### Jupyter Notebook

The primary analysis is conducted within the `wikispeedia.ipynb` notebook. Open this notebook using Jupyter to explore the following:

- **Data Parsing and Cleaning**: Understand how Wikipedia datasets are processed to construct the graph.
- **Shortest Path Analysis**: Learn how the Gurobi solver is applied to find the shortest paths between articles.
- **Longest Shortest Path Approximation**: Explore methods like random sampling and landmark-based approximations to analyze the graph's structure.

### Data Files

- **`articles.tsv`**: Contains the list of Wikipedia articles used in the analysis.
- **`links.tsv`**: Details the hyperlinks between the articles, forming the edges of the graph.

## File Structure

```
6-degrees-of-wikipedia/
│── articles.tsv           # List of Wikipedia articles
│── links.tsv              # Hyperlinks between articles
│── wikispeedia.ipynb      # Jupyter Notebook for analysis
│── requirements.txt       # Python dependencies
│── README.md              # Project documentation
```

## Dependencies

- **Python Packages**:
  - `numpy`
  - `pandas`
  - `networkx`
  - `matplotlib`
  - `gurobipy`
  - `jupyter`

  Install all dependencies using:

  ```bash
  pip install -r requirements.txt
  ```

- **Gurobi Optimizer**: Ensure that Gurobi is installed and properly configured.

## Contributing

Contributions to this project are welcome! To contribute:

1. **Fork the Repository**: Click on the "Fork" button at the top right corner of this page.
2. **Create a New Branch**: Use a descriptive name for your branch.

   ```bash
   git checkout -b feature-branch
   ```

3. **Commit Your Changes**: Provide clear and concise commit messages.

   ```bash
   git commit -m 'Description of feature or fix'
   ```

4. **Push to the Branch**:

   ```bash
   git push origin feature-branch
   ```

5. **Open a Pull Request**: Navigate to the original repository and click on "New Pull Request".

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

## Acknowledgments

- **Wikispeedia**: The original game that inspired this analysis.
- **Wikipedia**: For providing the datasets and the platform that makes this analysis possible.
- **Gurobi Optimizer**: For the powerful optimization tools used in this project.

For any questions or issues, please open an issue on GitHub or contact the repository owner.

```

This `README.md` provides a comprehensive overview of the project, including its purpose, setup instructions, usage guidelines, and contribution protocols. It ensures that users and contributors have clear and concise information to understand and engage with the project effectively. 
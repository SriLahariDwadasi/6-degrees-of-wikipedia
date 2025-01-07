# 6-degrees-of-wikipedia
Gurobi plays WikiSpeedia

In this project, we delve into the intricate world of network optimization using Wikipedia’s vast network
of articles and hyperlinks. Inspired by the game Wikispeedia, which challenges players to navigate
between Wikipedia articles through the shortest chain of links, our "6 Degrees of Wikipedia" project
analyzes the connectivity within Wikipedia through graph-based models. By parsing, decoding, and
cleaning the datasets, we construct a directed graph where articles are represented as nodes and links as
directed edges. This graph serves as the foundation for various analyses, including finding the shortest
paths and approximating the longest shortest paths within the network. We employ several optimization
models: a direct application of the Gurobi solver for the shortest path problem, random sampling for
identifying the longest shortest path, and a landmark-based approximation as an alternative approach.
Each model provides unique insights into the graph's structure, connectivity, and the potential "6 Degrees
of Separation" phenomenon, shedding light on the interplay between network topology and navigability.

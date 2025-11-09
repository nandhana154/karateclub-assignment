# Karate Club Community Detection  
Recursive Spectral Modularity – Graph Theory Project (DSC212)

This project applies **community detection** on the well-known *Zachary’s Karate Club* network.
The goal is to use graph structure to discover how the club naturally splits into groups.

We use **modularity maximization with spectral bisection**:
- Build the modularity matrix of the graph
- Compute the leading eigenvector
- Split the graph based on the sign of the eigenvector values
- Repeat the process recursively until modularity cannot improve

---

## What the code does

1. Loads the karate club graph from NetworkX  
2. Computes the modularity matrix for the current community  
3. Finds the leading eigenvector  
4. Divides nodes into two communities  
5. Repeats until no more meaningful splits exist  
6. Saves a visualization after every iteration

The visualizations generated during the process are stored in the `figures/` folder.

---

## Metrics Calculated

At every iteration, the following metrics are calculated for each node:
- Degree centrality
- Betweenness centrality
- Closeness centrality
- Clustering coefficient

This helps understand how important each node is inside the network.

---

## How to run

1. Clone this repository:
   ```sh
   git clone https://github.com/<your-username>/Karate-Club-Community-Detection.git
pip install networkx numpy matplotlib pandas
jupyter notebook karate_modularity_full.ipynb


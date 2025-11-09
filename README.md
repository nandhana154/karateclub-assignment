# karateclub-assignment
#  Community Detection on the Karate Club Graph  
**Spectral Modularity Based Recursive Bisection**

This project detects communities in **Zachary’s Karate Club network** using the concept of
**modularity maximization**. The goal is to use graph structure alone to reveal natural splits
in the network—without any prior knowledge of the actual groups.

---

##  What this project does

✔ Loads the karate club graph (34 nodes, 78 edges)  
✔ Computes the **modularity matrix**  
✔ Uses the **leading eigenvector** to perform community bisection  
✔ Repeats the process recursively while modularity improves  
✔ Saves graph visualizations at each iteration  

Each iteration generates a graph image showing how the community structure evolves.

---

##  Metrics computed for every iteration

For each split, the notebook calculates:

| Metric | What it tells us |
|--------|------------------|
| Degree Centrality | How many direct connections a node has |
| Betweenness | Whether a node lies on shortest paths (a communication controller) |
| Closeness | How quickly a node can reach others in the network |
| Clustering Coefficient | How tightly its neighbors are connected |

All of these help understand whether a node is **central or peripheral** during community formation.

---

## Project Structure

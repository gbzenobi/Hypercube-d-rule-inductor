**This model is still under experimentation, so any errors or mathematical dilemmas are open to discussion.**

---

Hypercube model characteristics.
* **Entropy-free**: Unlike what we expect to do in a decision tree, this model does not need to calculate any impurity metrics, entropy, pruning, among others.
* **not sensitive to initial conditions**: The set of rules it induces are initially deterministic in nature (although these may change if merged with another model, such as a genetic algorithm).
* **Noise-free**: If the assumptions are met, and the classification is correctly done then the boundaries delimited by the model will always be the same(unless the independent variables or classes change).
* **Rule inductor**: It generates well-defined(1-cube according to Petrie notation) regions in Euclidean space, forming a hypercube in a trivial classification problem and k-hypercubes when the problem involves non-trivial classification(e.g. in the case of k-clusters), this makes more sense when working in high dimensions and the data must be separated.
* **Predictor**: Once the rules are extracted it is possible to use them for classification and prediction, either by means of a tree or some brute force method.

---

Necessary assumptions: *Initially the experiments were performed on uniform distributions, however this does not imply that they cannot be applied to Gaussian distributions, or to more complex cases such as problems of elliptic or spherical nature. Studying the formulations and effects of high-dimensional geometries (such as regular convex polytopes) is fundamental to determine the scope and use cases of this model.*

---

## Topics covered

1. Brief history of how i designed the hypercube model
2. About hypercubes
3. Polytopes and convexity
4. Petrie notation and polygons
5. Introduction to the Hypercube D-rule inductor algorithm(and his elements).
6. General understanding of the Hypercube model
7. Dependencies
8. First approach to the model: rule extraction using the standard deviation and mean criteria.
9. Implementation of the hypercube D-rule inductor with the standard deviation and mean criterion.
10. Experiment on uniform and K-Means distributions with the standard deviation criterion and mean.
11. Implementation of the linearization criterion of dimensions
12. Uniform distribution experiment with the criterion of linearization of dimensions
13. Final update of the Hypercube D-rule inductor model; prediction method, accuracy and hypercube intersection ratio.
14. Experiment in R3 with intersection ratio and adaptive clustering
15. 5-dimensional final experiment; prediction function, time-series splitting with adaptive clustering and optimized rule extraction
16. Final comments and reflections.

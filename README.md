# Linear Time Algorithms for Finding and Testing Minimal d-Separators in Causal Graphs
## Overview  
This notebook provides a clear, step-by-step Python implementation of the linear-time algorithms for finding and testing **minimal d-separators** in causal graphs (DAGs, CPDAGs, RCGs, and AGs) as described by Van der Zander & Liśkiewicz (2020). All procedures run in \(O(n + m)\) time, where \(n\) is the number of nodes and \(m\) the number of edges. You’ll also find practical examples showing how d-separation underpins adjustment-set selection and conditional instrumental-variable identification in causal inference.  

## Usage  
1. **Open** `minimal_d_separators.ipynb` in Jupyter or JupyterLab.  
2. **Run the cells** in order to:  
   - Load and visualize example graphs  
   - Define and test `test_min_sep` and `find_min_sep` functions  
   - Benchmark performance on graph instances  

## Notebook Structure  
1. **Definitions**  
   - Recap of DAGs, CPDAGs, RCGs, AGs  
   - Formal definition of d-separation and minimality  
2. **Implementation**  
   - `test_min_sep(G, X, Y, Z, I, R)`: linear-time separator test  
   - `find_min_sep(G, X, Y, I, R)`: linear-time construction algorithm  
   - Core routines built on BFS and set intersections  
3. **Examples & Benchmarks**  
   - Sample graphs illustrating separator placement

---  
**Primary Reference**  
Van der Zander, B., & Liśkiewicz, M. (2020). *Finding Minimal d-Separators in Linear Time and Applications*. Proceedings of the 35th Uncertainty in Artificial Intelligence Conference (UAI 2019), *Proceedings of Machine Learning Research*, 115:637–647.  
Available at: https://proceedings.mlr.press/v115/van-der-zander20a.html
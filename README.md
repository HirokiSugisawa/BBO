# BBO (Batch Bayesian Optimization)
This is a program related to the generation of initial 24 points, batch Bayesian optimization, and the surrogate model construction, as presented in the following paper.
Y. Tanabe, H. Sugisawa, T. Miyazawa, K. Hotta, K. Shiratori, T. Fujitanib, 
"High-Throughput Optimization of a High-Pressure Cata-lytic Reaction,"
Journal of ... (2025)

## Library
pandas, numpy, scipy, matplotlib, scikit-learn, jupyterlab

## Contents
To reproduce the results, the source code and dataset are stored in the scr folder. Descriptions of each program are given below. Basically, you can reproduce the paper by executing the programs in numerical order.

### 1. Initial Guess Generation
Using the first_10.dat file, 24 points for the initial experiment are generated. 
To ensure spatial diversity of the experimental points, the D-optimality criterion is applied.

### 2. BBO for Composition
This is the BBO algorithm for optimizing catalyst composition. In this study, the Kriging method is used; however, the Thompson method is also implemented and available for use.

### 3. Surrogate Model Construction
This is the algorithm for constructing a surrogate model.

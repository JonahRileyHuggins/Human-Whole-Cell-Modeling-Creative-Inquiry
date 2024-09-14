# Background

Modeling events for predictive purposes broadly has two avenues: descriptive and emperical. The former primarily uses population level data and statistical learning methods to discern both features and predictions from a dataset. Regression, classification, and Tree-Based methods are all common approaches to statistical learning [1]. The latter uses relationships between individual components within an environment to draw mechanistic reasoning (i.e. prediction with full clarity over time on how each component contributes). A common application of such work is Kinetic Modeling, which represent the dynamics of a system in response to perturbations (i.e. treatments, etc.)[2]. Kinetic models are often used to model biochemical signaling networks, which can be essential towards understanding and predicting such network's influence on living cells. 

SPARCED, a lar. ge-scale mechanistic model is a great example of this, comprising 924 components and over 2900 reactions defined within pathways commonly disregulated in cancer cells.

 Further, SPARCED has a secondary modeling framework for representing (stochastic) gene expression within cells. Stochastic gene expression. [More On Stochastic Element Module]. In sequential process; our kinetic model begins the simulation process for 30 simulation seconds (i.e. not real time). The kinetic model then sends protein, mRNA, and gene information to the gene expression module, that adds a level of stochasticity (or randomness) to these component concentrations. These values are used as the initial starting points of the next simulation round, and this proceeds until the total length of simulation time is finished.

The first representation of this model was published in 2018 as a closed source software implementation in MATLAB, however since has been adapted to a Python framework with simulation tools leveraging the speed and efficiency of C++ with easier usability of Python. 

Current

modeling

SPARCED

- What is it
  - Kinetic models
  - Capabilities
  - Components
    - Stochastic Gene expression module
    - Stochastic / Deterministic hybrid kinetic model


References:

1. An introduction to statistical learning with applications in R
2. Kinetic Models of BioChemical Signaling Events - MRB & MB

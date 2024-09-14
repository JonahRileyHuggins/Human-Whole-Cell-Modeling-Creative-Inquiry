# Welcome

The purpose of this repository is to serve as a hub where interested researchers are able to learn the basics of mechanistic modeling in Python, as well as an introduction to ongoing tasks and projects surrounding the SPARCED model: a large-scale mechanistic model of cancer signaling pathways. After finishing the modules, readers should have the basic knowledge required to operate and work with the SPARCED model. We do not intend for this page to be a comprehensive guide to the systems biology modeling, rathe, we hope this will serve as a self-contained roadmap for future researchers to familiarize themselves with the model efficiently and begin to run SPARCED simulations independently.

Students interested in Creative Inquiry projects involving SPARCED should have a high interest to learn both concepts of molecular cell biology and computer science. There is no expectation that students have formal classwork in either, just a willingness to learn! Before committing to credit hours, it is requested that students complete Modules 0-3 here, return the completed work as proof of completion, and email jrhuggi@g.clemson.edu to get involved.

### Modules:

These modules serve as a learning resource for interested students to feel comfortable with the tools and concepts essential towards mechanistic modeling in Python.


```{toctree}
:maxdepth: 2
:caption: Contents:

Module 0 - Project Background(s).md
Module 1 - Python and Jupyter Notebooks Primer.ipynb
Module 2 - Packages - Working Environments - and Command Line Operations.ipynb
Module 3 - Modeling with Tellurium and Antimony.ipynb
```



* Module 0 represents an informative background on the SPARCED model itself
* Module 1 is a brief walkthrough on using python
* Module 2 dives into package installation and working environments
* Module 3 Shows the core concepts of modeling kinetic events in Python

Future planned (non-required) modules:

* The basics of operating the SPARCED model
* Message Passing Interface and parallelization for increased efficiency
* Coding Standards, Clean Code, and Unit Testing
* Validating model expansions with the internal benchmarking pipeline

### Project One: Model Expansion Through Pathway Integration (Model Merging)

Mechanistic models can make accurate predictions given the relationships between components, however, this necessitates that the relationships of components be thoroughly described in detail. To this end, we look to identify and integrate already existing models (preferentially Ordinary Differential Equation or SBML formats) of canonical cell pathways. Researchers contributing here will identify candidate models, verify their operation and validity, and merge the components with the SPARCED model. See the figure below for a roadmap towards pathway integration.

![1724969845278](image/README/1724969845278.png)

### Project Two: Constructing a Stochastic Gene Expression Module Representing The Complete Human Genome

Currently, SPARCED has functionality to represent 141 of the roughly 20,000 functional protein-encoding genes within the human genome. Leveraging the ubiquity of available databases (ENSEMBL, Hugo Gene Nomenclature Ontology, etc.), a realistic goal of this project is to construct a dataset comprising the expression and degredation information critical for representing whole-genome level stochastic gene expression. Ideally, since we already have tools for recontextualizing our existing large-scale model of a cell (SPARCED), we could readily transition cells types to test it's predictive capabilities in a variety of settings.

### Project Three: A Repository Of Available And Validated Pathway Models

Systems biology is littered with disparate pathway models of various formats (ODE-based, SBML, R, MATLAB, Julia). While useful for their particular context, they lose relevance to the broader community due to a lack of interoperability with other modeling tools. Further, despite existing, convenient, and well-curated databases of biological models (BioModels) and standards detailing construction and format (SBML), broad adoption from the systems biology community has not yet been acheived. This leaves a need to **A)** determine the extent of cellular pathway models of a broad variety that might have potential relevance for a human WCM, and **B)** curate them into a defined format (SBML) such that they can be uploaded to BioModels. Students involved on this project will primarily use web-scraping data storage techniques, such as programmatic interaction with APIs and data management, to identify, gather, and curate existing models. Potentially other data science techniques in the construction of said database will be used as the project gets a footing.

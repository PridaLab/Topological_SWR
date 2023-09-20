# Topological_SWR

Characterization of hippocampal sharp-wave ripples (SWR) using Topological Data Analysis. 

TopologicalRippleClassification.ipynb is a jupyter notebook with an example of the code used for this project.

This notebook illustrates the pipeline of the topological analysis of SWR. Given that some parts of the code are computationally expensive, we provide pre-computed results in a file. If you are interested in either testing your own data or check the computation of the provided dataset you can execute the corresponding part locally.

The pipeline consists in different steps involving different topological analysis. The first step is to compute Persistent Homology barcodes over the dataset to know about its components, holes and cavities.

![alt text](images/example_barcodes.png)

In this case we see we have only one continuous component without holes or cavities.

Next step is to visualize how our dataset features project over the point cloud using dimensionality reduction.

![alt text](images/example_embeddings.png)

Finally we can quantify how structured are these features over the point cloud in any space with an arbitrary number of dimensions using our tool, the Structure Index (https://github.com/PridaLab/structure_index.git).

![alt text](images/example_SI.png)

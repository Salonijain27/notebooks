# RAPIDS Notebooks
## Intro
These notebooks provide examples of how to use RAPIDS libraries, like cuML and cuGraph.  These notebooks are designed to be self contained with the [RAPIDS Docker Container](https://hub.docker.com/r/rapidsai/rapidsai/) and [RAPIDS Nightly Docker Containers](https://hub.docker.com/r/rapidsai/rapidsai-nightly) and can run on airgapped systems.  You can quickly get this continaer using the install guide from the [RAPIDS.ai Getting Started page](https://rapids.ai/start.html#get-rapids)

### More notebooks in [Notebooks Contrib Repo](https://github.com/rapidsai/notebooks-contrib)
For additional, community driven notebooks, which will include our blogs, tutorials, workflows, and more intricate examples, please see the [Notebooks Contrib Repo](https://github.com/rapidsai/notebooks-contrib).  These notebooks use generally use real world data sets.

If you want to include these notebooks with your RAPIDS Docker pull's Jupyter Lab, [please follw these instructions](https://github.com/rapidsai/notebooks-contrib/blob/master/BUILD.md).   

If you're using Conda, you can just `git clone https://github.com/rapidsai/notebooks-contrib.git` 

## RAPIDS Notebooks and Utilities

### XGBoost Notebook
| Folder    | Notebook Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| XGBoost   | [XGBoost Demo](xgboost/XGBoost_Demo.ipynb)           | This notebook shows the acceleration one can gain by using GPUs with XGBoost in RAPIDS.                                                                                                                                       |
### CuML Notebooks
 The cuML notebooks showcase how to use the machine learning algorithms implemented in cuML along with the advantages of using cuML over scikit-learn. These notebooks compare the time required and the performance of the algorithms. Below are a list of such algorithms:

| Folder    | Notebook Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| cuML      | [Coordinate Descent](cuml/coordinate_descent_demo.ipynb)     | This notebook includes code examples of lasso and elastic net models. These models are placed together so a comparison between the two can also be made in addition to their sklearn equivalent.                                                                                                                                                                |
| cuML      | [DBSCAN Demo](cuml/dbscan_demo.ipynb)            | This notebook showcases density-based spatial clustering of applications with noise (dbscan) algorithm using the `fit` and `predict` functions                                                                              |
| cuML      | [Forest Inference](cuml/forest_inference_demo.ipynb)   | This notebook shows how to use the forest inference library to load saved models and perform prediction using them. In addition, it also shows how to perform training and prediction using xgboost and lightgbm models.|
| cuML      | [HoltWinters Demo](cuml/holtwinters_demo.ipynb)  | This notebook includes code example for the holt-winters algorithm and it showcases the `fit` and `forecast` functions.                 |
| cuML      | [K-Means Demo](cuml/kmeans_demo.ipynb) | This notebook includes code example for the k-means algorithm and it showcases the `fit` and `predict` functions.                                                                                                                                             |
| cuML      | [K-Means MNMG Demo](cuml/kmeans_demo-mnmg.ipynb) | This notebook includes code example for the k-means multi-node multi-GPU algorithm and it showcases the `fit` and `predict` functions.                                                                                                                                             |
| cuML      | [Linear Regression Demo](cuml/linear_regression_demo.ipynb) | This notebook includes code example for linear regression algorithm and it showcases the `fit` and `predict` functions.                                                                                                                                             |
| cuML      | [Metrics Demo](cuml/metrics_demo.ipynb) | This notebook includes code examples showcasing the different metrics provided in cuML. The results are compared with their scikit learn counterparts.                                                                                                                                             |
| cuML      | [Mini Batch SGD Demo](cuml/mini_batch_sgd_demo.ipynb) | This notebook includes code example for mbsgd classifier and regressor algorithms and it showcases their `fit` and `predict` functions.                                                                                                                                             |
| cuML      | [Nearest Neighbors_demo](cuml/nearest_neighbors_demo.ipynb)               | This notebook showcases k-nearest neighbors (knn) algorithm using the `fit` and `kneighbors` functions                                                                                                                          |
| cuML      | [PCA Demo](cuml/pca_demo.ipynb)               | This notebook showcases principal component analysis (PCA) algorithm where the model can be used for prediction (using `fit_transform`) as well as converting the transformed data into the original dataset (using `inverse_transform`).                                                                                                                |
| cuML      | [Random Forest Classification and Pickling](cuml/random_forest_demo.ipynb)   | Demonstrates how to fit cuML and scikit-learn Random Forest Classification models. Then we save the cuML model for future use with Python's pickling mechanism and demonstrate how to re-load it for prediction.|
| cuML      | [Random Forest Multi-node / Multi-GPU](cuml/random_forest_mnmg_demo.ipynb)   | Demonstrates how to fit Random Forest models using multiple GPUs via Dask. |
| cuML      | [Ridge Regression Demo](cuml/ridge_regression_demo.ipynb)  | This notebook includes code examples of ridge regression and it showcases the `fit` and `predict` functions.                                                                                                                                          |
| cuML      | [SGD_Demo](cuml/sgd_demo.ipynb)               | The stochastic gradient descent algorithm is demonstrated in the notebook using `fit` and `predict` functions                                                                        |
| cuML      | [SVM_Demo](cuml/svm_demo.ipynb)               | Binary Support Vector Machine classification is demonstrated in this notebook using `fit` and `predict` functions. |
| cuML      | [TSNE_Demo](cuml/tsne_demo.ipynb)               | In this notebook, T-Distributed Stochastic Neighborhood Embedding is demonstrated applying the Barnes Hut method on the Fashion MNIST dataset using our `fit_transform` function                                                                      |
| cuML      | [TSVD_Demo](cuml/tsvd_demo.ipynb	)              | This notebook showcases truncated singular value decomposition (tsvd) algorithm which like PCA performs both prediction and transformation of the converted dataset into the original data using `fit_transform` and `inverse_transform` functions respectively                                                                                                     |
| cuML      | [UMAP_Demo](cuml/umap_demo.ipynb)              | The uniform manifold approximation & projection algorithm is compared with the original author's equivalent non-GPU Python implementation using `fit` and `transform` functions                       |
| cuML      | [UMAP_Demo_Graphed](cuml/umap_demo_graphed.ipynb)      | Demonstration of cuML uniform manifold approximation & projection algorithm's supervised approach against mortgage dataset and comparison of results against the original author's equivalent non-GPU \Python implementation. |
| cuML      | [UMAP_Demo_Supervised](cuml/umap_supervised_demo.ipynb)   | Demostration of UMAP supervised training.  Uses a set of labels to perform supervised dimensionality reduction. UMAP can also be trained on datasets with incomplete labels, by using a label of "-1" for unlabeled samples. |


### CuDF Notebooks
| Folder    | Notebook Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| cuDF      | [notebooks_Apply_Operations_in_cuDF](cudf/notebooks_Apply_Operations_in_cuDF.ipynb)            | This notebook showcases two special methods where cuDF goes beyond the Pandas library: apply_rows and apply_chunk functions. They utilized the Numba library to accelerate the data transformation via GPU in parallel.                                                                            |
| cuDF      | [notebooks_numba_cuDF_integration](cudf/notebooks_numba_cuDF_integration.ipynb)               | This notebook showcases how to use Numba CUDA to accelerate cuDF data transformation and how to step by step accelerate it using CUDA programming tricks                                                                                                                          |

<<<<<<< HEAD
<<<<<<< HEAD
## CuGraph Notebooks
| Folder    | Notebook Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| cuGraph   | [BFS](cugraph/BFS.ipynb)                    | Demonstration of using cuGraph to computer the Bredth First Search space from a given vertex to all other in our training graph                                                                                               |
| cuGraph   | [Connected Components](cugraph/ConnectedComponents.ipynb)      | Demonstration of using cuGraph to compute weakly and strongly connected components in a test graph.                                                                                                                  |
| cuGraph   | [Louvain](cugraph/Louvain.ipynb)                | Demonstration of using cuGraph to identify clusters in a test graph using the Louvain algorithm                                                                                                                               |
| cuGraph   | [Pagerank](cugraph/Pagerank.ipynb)               | Demonstration of using both NetworkX and cuGraph to compute the PageRank of each vertex in our test dataset                                                                                                                   |
| cuGraph   | [Renumber](cugraph/Renumber.ipynb)               | Demonstrate of using the renumbering features to assigned new vertex IDs to the test graph.  This is useful for when the data sets is  non-contiguous or not integer values                                                   |
| cuGraph   | [SSSP](cugraph/SSSP.ipynb)                   | Demonstration of using cuGraph to computer the The Shortest Path from a given vertex to all other in our training graph                                                                                                       |
| cuGraph   | [Spectral-Clustering](cugraph/Spectral-Clustering.ipynb)    | Demonstration of using cuGraph to identify clusters in a test graph using Spectral Clustering using both the (A) Balance Cut and (B) the Modularity Maximization quality metrics                                              |
| cuGraph   | [Triangle Counting](cugraph/Triangle-Counting.ipynb)      | Demonstration of using both NetworkX and cuGraph  to compute the the number of Triangles in our test dataset                                                                                                                  |
| cuGraph   | [Vertex-Similarity](cugraph/Vertex-Similarity.ipynb)      | Demonstration of using cuGraph to compute vertex similarity using both the Jaccard Similarity and the Overlap Coefficient.                                                                                                    |
| cuGraph   | [Weighted-Jaccard](cugraph/Weighted-Jaccard.ipynb)       | Demonstration of using cuGraph to compute the Weighted Jaccard Similarity metric on our training dataset.                                                                                                                     |

## Tutorial with an End to End workflow
=======
=======
>>>>>>> bcdac1526bd1a0a2ac5f630cc0330cd2a82f40d7
### CuGraph Notebooks

| Folder  | Notebook Title                                               | Description                                                  |
| ------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| cuGraph -> centrality| [Katz](cugraph/centrality/Katz.ipynb)                        | Compute the Katz centrality for every vertex                 |
| cuGraph -> community| [Louvain](cugraph/community/Louvain.ipynb)                   | Demonstration of using cuGraph to identify clusters in a test graph using the Louvain algorithm |
| cuGraph -> community| [Spectral-Clustering](cugraph/community/Spectral-Clustering.ipynb) | Demonstration of using cuGraph to identify clusters in a test graph using Spectral Clustering using both the (A) Balance Cut and (B) the Modularity Maximization quality metrics |
| cuGraph -> community| [Subgraph Extraction](cugraph/community/Sungraph-Extraction.ipynb) | Compute a subgraph of the existing graph including only the specified vertices |
| cuGraph -> community| [Triangle Counting](cugraph/community/Triangle-Counting.ipynb) | Demonstration of using both NetworkX and cuGraph  to compute the the number of Triangles in our test dataset |
| cuGraph -> components| [Connected Components](cugraph/components/ConnectedComponents.ipynb) | Find weakly and strongly connected components in a graph     |
| cuGraph -> cores| [K-Core](cugraph/cores/kcore.ipynb)                          | Extracts the K-core cluster                                  |
| cuGraph -> cores | [Core Number](cugraph/cores/core-number.ipynb)               | Computer the Core number for each vertex in a graph          |
| cuGraph -> link_analysis | [Pagerank](cugraph/link_analysis/Pagerank.ipynb)             | Demonstration of using both NetworkX and cuGraph to compute the PageRank of each vertex in our test dataset |
| cuGraph -> link_prediction | [Jacard Similarity](cugraph/link_prediction/Jaccard-Similarity.ipynb) | Compute vertex similarity score using both:<br />- Jaccard Similarity<br />- Weighted Jaccard |
| cuGraph -> link_prediction | [Overlap Similarity](cugraph/link_prediction/Overlap-Similarity.ipynb) | Compute vertex similarity score using the Overlap Coefficient |
| cuGraph -> traversal| [BFS](cugraph/traversal/BFS.ipynb)                           | Demonstration of using cuGraph to computer the Breadth First Search space from a given vertex to all other in our training graph |
| cuGraph -> traversal | [SSSP](cugraph/traversal/SSSP.ipynb)                         | Demonstration of using cuGraph to computer the The Shortest Path from a given vertex to all other in our training graph |
| cuGraph -> structure| [Renumber](cugraph/structure/Renumber.ipynb)                 | Demonstrate of using the renumbering features to assigned new vertex IDs to the test graph.  This is useful for when the data sets is  non-contiguous or not integer values |
| cuGraph -> structure| [Symmetrize](cugraph/structure/Symmetrize.ipynb)             | Symmetrize the edges in a graph                              |

### Tutorial with an End to End workflow
<<<<<<< HEAD
>>>>>>> 398c31c85730779d3daa28128b03caf298e03677
=======
>>>>>>> bcdac1526bd1a0a2ac5f630cc0330cd2a82f40d7

| Folder    | Notebook Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Tutorials | [DBSCAN_demo_full](tutorials/DBSCAN_Demo_Full.ipynb)       | Demonstration of how to use DBSCAN - a popular clustering algorithm - and how to use the GPU accelerated implementation of this algorithm in RAPIDS.                                                                               |
| Tutorials | [HoltWinters_demo_full](tutorials/holtwinters_demo_full.ipynb)   | Demonstration of how to use Holt-Winters, a time-series forecasting algorithm, on a dataset to make GPU accelerated out-of-sample predictions.      |

### Utils Scripts
| Folder    | Script Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| utils     | dask-cluster.py        | launches a configured Dask cluster (a set of nodes) for use within a notebook                                                                                                                                                 |
| utils     | dask-setup.sh          | a low-level script for constructing a set of Dask workers on a single node                                                                                                                                                    |
| utils     | dask.conf          | a Dask user configuration and settings file for the RAPIDS docker container                                                                                                                                                    |
| utils     | split-data-mortgage.sh | splits mortgage data files into smaller parts, and saves them for use with the mortgage notebook                                                                                                                              |
| utils     | start-jupyter.sh       | starts a JupyterLab environment for interacting with, and running, notebooks                                                                                                                                                  |
| utils     | stop-jupyter.sh        | identifies all process IDs associated with Jupyter and kills them                                                                                                                                                             |

### Documentation
| Folder    | Document Title         | Description                                                                                                                                                                                                                   |
|-----------|------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| docs      | ngc-readme             |                                                                                                                                                                                                                               |
| docs      | dockerhub-readme       |                                                                                                                                                                                                                               |

## Additional Information
* The `cuml` folder also includes a small subset of the Mortgage Dataset used in the notebooks and the full image set from the Fashion MNIST dataset.

* `utils`: contains a set of useful scripts for interacting with RAPIDS
<<<<<<< HEAD
<<<<<<< HEAD

* For additional, community driven notebooks, which will include our blogs, tutorials, workflows, and more intricate examples, please see the [Notebooks Contrib Repo](https://github.com/rapidsai/notebooks-contrib)
=======
>>>>>>> 398c31c85730779d3daa28128b03caf298e03677
=======
>>>>>>> bcdac1526bd1a0a2ac5f630cc0330cd2a82f40d7

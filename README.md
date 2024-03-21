# Search ANN Benchmark

Benchmark the search performance of Approximate Nearest Neighbor (ANN) algorithms implemented in various systems.
This repository contains notebooks and scripts to evaluate and compare the efficiency and accuracy of ANN searches across different platforms.

## Introduction

Approximate Nearest Neighbor (ANN) search algorithms are essential for handling high-dimensional data spaces, enabling fast and resource-efficient retrieval of similar items from large datasets.
This benchmarking suite aims to provide an empirical basis for comparing the performance of several popular ANN-enabled search systems.

## Prerequisites

Before running the benchmarks, ensure you have the following installed:

- Docker
- Python 3.10 or higher

## Setup Instructions

1. **Prepare the Environment:**

    Create directories for datasets and output files, then download the necessary datasets using the provided script.

    ```bash
    mkdir -p dataset output
    /bin/bash ./download.sh
    ```

2. **Install Dependencies:**

    Install all required Python libraries.

    ```bash
    pip install -r requirements.txt
    ```

## Benchmark Notebooks

The repository includes the following Jupyter notebooks for conducting benchmarks:

- [Elasticsearch](run-elasticsearch.ipynb)
- [OpenSearch](run-opensearch.ipynb)
- [Qdrant](run-qdrant.ipynb)
- [Vespa](run-vespa.ipynb)
- [Weaviate](run-weaviate.ipynb)

Each notebook guides you through the process of setting up the test environment, loading the dataset, executing the search queries, and analyzing the results.

## Contributing

We welcome contributions!
If you have suggestions for additional benchmarks, improvements to existing ones, or fixes for any issues, please feel free to open an issue or submit a pull request.

## License

This project is licensed under the Apache License 2.0.


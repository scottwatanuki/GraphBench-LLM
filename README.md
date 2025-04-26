# GraphBench-LLM

A benchmarking framework for evaluating large language models (LLMs) on graph theory problems.

## Overview

GraphBench-LLM evaluates the capabilities of leading LLMs in solving fundamental graph theory problems. This benchmark assesses model performance across several graph-theoretic tasks with varying computational complexity, from basic properties like connectivity to NP-complete problems like finding maximum cliques.

## Models Evaluated

- GPT-4o (OpenAI)
- DeepSeek v3
- Gemini Flash 2.0
- DeepThink R1

## Benchmark Tasks

The benchmark evaluates models on five key graph theory tasks:
- **Maximum Degree**: Finding the highest number of edges connected to a single vertex
- **Connectivity**: Determining if the graph is connected
- **Bipartiteness**: Determining if the graph can be divided into two disjoint sets
- **Hamiltonian Cycle**: Determining if the graph contains a cycle visiting each vertex exactly once
- **Maximum Clique**: Finding the size of the largest complete subgraph

## Dataset

The benchmark dataset is available in [graph_benchmark_dataset.csv](graph_benchmark_dataset.csv), containing various graph problems with verified ground truth answers.

## Analysis

The analysis is implemented in two Jupyter notebooks:
- [GraphBenchmark.ipynb](GraphBenchmark.ipynb): Contains the core benchmarking implementation
- [GraphBenchmark_Analysis.ipynb](GraphBenchmark_Analysis.ipynb): Analyzes and visualizes the benchmark results

## Key Findings

The analysis examines:
- Performance across different computational complexity tasks
- Impact of graph size and density on model accuracy
- Error patterns and systematic biases in model responses
- Correlation between theoretical complexity and model performance

## Visualizations

The repository includes several visualizations:
- [graph_size.png](results/graph_size.png): Model performance by graph size
- [graph_density.png](results/graph_density.png): Model performance by graph density
- [max_degree_errors.png](results/max_degree_errors.png): Error distribution for maximum degree task
- [max_clique_errors.png](results/max_clique_errors.png): Error distribution for maximum clique task
- [model_performance.png](results/model_performance.png): Overall model performance comparison

## Usage

To run the analysis:

```python
# Clone the repository
git clone https://github.com/yourusername/GraphBench-LLM.git
cd GraphBench-LLM

# Install dependencies
pip install pandas numpy matplotlib seaborn jupyter

# Run the analysis notebook
jupyter notebook GraphBenchmark_Analysis.ipynb
```

## Citation

If you use this benchmark in your research, please cite:

```
@misc{GraphBenchLLM2025,
  author = {Alexander Divoux, Jae Young Beck, Scott Watanuki},
  title = {GraphBench-LLM: Benchmarking Large Language Models on Graph Theory Problems},
  year = {2025},
  publisher = {GitHub},
  url = {https://github.com/scottwatanuki/GraphBench-LLM}
}
```

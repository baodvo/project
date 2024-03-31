# Node and Edge Attributes Graph Neural Networks for Cascading Failure Prediction in Power Grids

This repository contains datasets and code for the paper "Cascading Failure Prediction in Power Grid Using Node and Edge Attributed
Graph Neural Networks"

## Cascading failure simulation
We use an AC-based cascading failure simulation model described in: \
Noebels, M., Preece, R., Panteli, M. "AC Cascading Failure Model for Resilience Analysis in Power Networks." IEEE Systems Journal (2020).\
We thank the authors of AC-CFM for making their code publicly available.

## Data Modeling
We use IEEE test cases with 39-bus and 118-bus as the network topology to simulate cascading failures. The simulation results are included in the `data` folder. For details about feature selection and data pre-processing, please refer to `data.py`.

## Installation
Refer to `requirements.txt` to reproduce the environment.

## Run GNN model
The main code to load the pre-processed dataset and train a GNN model is in `main.py`. Refer to `layer.py` for the implementation of the convolution layers dicussed in the paper.\
Choose GNN models from:
1. NEA_GNN
2. GCN  
3. GraphSAGE 
4. GIN 
5. GAT (GAT-A in paper)
6. GATE (GAT-B in paper)

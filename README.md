# Diffusing_Heat

This repository contains the dataset for the paper "Diffusing Heat: Generative Scan Path Optimization for Laser Powder Bed Fusion". The dataset is designed to train and evaluate generative models for optimizing scan paths and managing heat diffusion in the Laser Powder Bed Fusion (LPBF) process.

The provided dataset consists of two main splits: a training set containing 30,000 optimized scan path sequences, and a testing set containing 100 sequences used for model evaluation.

The data is saved in PyTorch's .pt format and is split into multiple batch files. Each data sample provides comprehensive information required for neural network processing, padded to a consistent sequence length. This includes the 2D normalized coordinates of the physical print blocks (coords), as well as a boolean mask matrix (mask) used to distinguish valid physical nodes from padded ones. Most importantly, each sample contains the ground-truth adjacency matrix (adj) representing the optimized closed-loop scan path. For completeness, the dataset also provides the global identifiers for each block (ids), the exact integer count of valid nodes in the sequence (num_nodes), and the calculated fitness score of that specific generated sequence (r_score).

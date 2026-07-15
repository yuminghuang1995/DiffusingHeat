# Diffusing_Heat

This repository contains the dataset for the project "Diffusing Heat". The dataset is designed to train and evaluate generative models for optimizing scan paths and managing heat diffusion in the Laser Powder Bed Fusion (LPBF) process.

The provided dataset consists of a testing dataset containing 2000 sequences used for model evaluation.

The data is saved in PyTorch's .pt format and is split into multiple batch files. Each data sample provides comprehensive information required for neural network processing, padded to a consistent sequence length. This includes the 2D normalized coordinates of the physical print blocks, as well as a boolean mask matrix used to distinguish valid physical nodes from padded ones. Most importantly, each sample contains the ground-truth adjacency matrix representing the optimized closed-loop scan path. For completeness, the dataset also provides the global identifiers for each block, the exact integer count of valid nodes in the sequence, and the calculated score of that specific generated sequence.

The results folder displays some testing results.

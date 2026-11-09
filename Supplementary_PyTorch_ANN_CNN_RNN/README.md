# Supplementary PyTorch Practical – ANN, CNN, and RNN

This material is **additional knowledge** for ML6402.

The main deep-learning implementation in the course remains **TensorFlow/Keras**. This supplementary notebook introduces PyTorch because it is widely used in machine-learning research and gives students a more explicit view of the training process.

## Coverage

- PyTorch tensors
- automatic differentiation
- CPU/GPU device selection
- TensorDataset and DataLoader
- nn.Module
- forward pass
- loss functions
- optimizers
- backpropagation
- reusable training/evaluation loops
- ANN example
- CNN example
- RNN example
- brief RNN-to-LSTM extension
- prediction
- saving and loading state dictionaries

The examples use Scikit-Learn built-in datasets or generated data, so **no external dataset path is required**.

## Requirement

```bash
pip install torch torchvision
```

When the full ML6402 environment is installed from the repository's `environment.yml`, PyTorch is included automatically.

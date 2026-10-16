# 25-20-10 Neural Network

A feedforward neural network that classifies digits represented as 5×5 binary grids using a 25-20-10 architecture.

## Overview

Each digit is represented by a 5×5 grid containing 25 pixels. Each pixel is binary:

- `1` = ON
- `0` = OFF

The network takes the 25 pixel values as input and predicts which digit, from 0 through 9, the grid represents.

## Architecture

| Layer | Neurons | Purpose |
|---|---:|---|
| Input | 25 | Receives the flattened 5×5 grid |
| Hidden | 20 | Learns patterns in the input |
| Output | 10 | Produces a score for each digit, 0–9 |

**Data flow:** 5×5 grid → 25 inputs → 20 hidden neurons → 10 outputs → predicted digit.

## Example Input

Example binary pattern representing the digit 7:

```text
1 1 1 1 1
0 0 0 0 1
0 0 0 1 0
0 0 1 0 0
0 1 0 0 0
```

The grid is flattened into a vector of 25 values before being passed into the network.

## Classification Process

1. Encode a digit as a 5×5 binary grid.
2. Flatten the grid into 25 input values.
3. Pass the values through the hidden layer.
4. Calculate the ten output scores.
5. Choose the highest-scoring output as the predicted digit.
6. Compare predictions with known labels during evaluation.

## Project Goals

- Understand feedforward neural networks.
- Explore how a network learns binary patterns.
- Implement or experiment with forward propagation and backpropagation.
- Train the model to classify ten numerical classes.
- Measure performance using labeled examples.
- Investigate how weights, biases, activation functions, and training parameters affect results.

## Evaluation

Evaluate the model on labeled examples that were not used for training. Useful metrics include:

- Overall classification accuracy
- Per-digit accuracy
- Confusion matrix
- Training and validation loss

Actual performance depends on the implementation and training data. Results will be added after they are measured.

## Status

Early-stage project. The implementation, dataset, training process, and measured results will be documented as development progresses.

## Future Improvements

- Build a complete training pipeline.
- Add labeled 5×5 digit patterns.
- Visualize input grids and predictions.
- Track training loss and accuracy.
- Test robustness to altered or noisy patterns.
- Compare architectures and activation functions.

## License

No license has been selected yet. Until a license is added, normal copyright applies to this repository's contents.

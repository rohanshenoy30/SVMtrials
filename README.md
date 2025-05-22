# SVMtrials

Experimenting with the different types of kernels on an SVM on the iris dataset.

## How to Choose the Right Kernel:

- Start with **linear kernel** for high-dimensional or sparse data (e.g., text classification).
- Use **RBF** when you suspect complex, nonlinear relationships but don’t know the exact nature.
- Try **polynomial** if you believe feature interactions of a specific degree are important.
- Use **grid search or cross-validation** to compare performance across kernels.

## Summary Table

| Kernel Type    | Formula                          | Captures Nonlinearity | Typical Use Case                                     |
|----------------|----------------------------------|------------------------|------------------------------------------------------|
| Linear         | xᵀx′                             | ❌                     | High-dimensional, linearly separable data            |
| Polynomial     | (xᵀx′ + c)ᵈ                      | ✅                     | When data has polynomial relationships              |
| RBF (Gaussian) | exp(−γ‖x − x′‖²)                | ✅✅                   | Most general-purpose, nonlinear datasets             |
| Sigmoid        | tanh(αxᵀx′ + c)                  | ✅                     | Experimental; neural network-like behavior           |


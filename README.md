# AIP2_2026S
Working repository for UNIST Introduction to Artificial Intelligence Programming 2

## Dependency of each lab sessions

## Lab Session Dependency Map

```
Lab 0: Environment & Python OOP
│   uv, Jupyter, classes, NumPy basics
│
└── Lab 1: Linear Algebra & GPU Tensors
    │   NumPy matmul, einsum, PyTorch tensors, CPU/GPU benchmark
    │
    ├── Lab 2: Linear Regression ──────────────────────────────┐
    │   │   Dataset pipeline, MSE loss, normal eq., grad. desc. │
    │   │                                                        │
    │   ├── Lab 3: Logistic Regression                          │
    │   │   │   Sigmoid, BCE loss, Ridge/Lasso, reuses Lab 2    │
    │   │   │                                                    │
    │   │   └── Lab 4: Softmax Classification                   │
    │   │               │   log-sum-exp, cross-entropy, MNIST   │
    │   │               │                                        │
    │   │               └── Lab 5: SVM & Optimizer Class        │
    │   │                           Hinge loss, SGD/Momentum    │
    │   │                           custom Optimizer base class  │
    │   │                                   │                    │
    │   └───────────────────────────────────┼────────────────────┘
    │                                       │  (training pipeline
    │                                       │   + optimizer reuse)
    │                                       ▼
    └──────────────────────────────► Lab 6: MLP & Backprop [PIVOT]
                                    │   Manual backward(), Module,
                                    │   Linear, ReLU from scratch
                                    │   verify vs. nn.Linear + autograd
                                    │
                                    └── Lab 7: Normalization & DataLoader
                                        │   RMSNorm/BatchNorm, custom
                                        │   Dataset/DataLoader (yield),
                                        │   experiment plotting
                                        │
                                        ├── Lab 8: CNN from Scratch
                                        │   │   Manual Conv2d, filter viz,
                                        │   │   reuses Module from Lab 6
                                        │   │
                                        │   └── Lab 9: ResNet
                                        │               ResidualBlock,
                                        │               gradient norm plots,
                                        │               CIFAR-10 benchmark
                                        │                       │
                                        └───────────────────────┘
                                                    │
                                                    ▼
                                            Lab 10: Transformer & MicroGPT
                                                Self-attention (Q,K,V),
                                                causal masking, pos. encoding,
                                                Transformer decoder block,
                                                character-level LM training
```
# Schedule

## Monday: Foundations of Deep Learning

- **11:00 – 13:00: Introduction to Deep Learning (Lecture)**
  - The Deep Learning Revolution & Motivation
  - Deep Learning Primitives: Architectures & Activations
    - Neural Network Architectures: From the Perceptron to MLPs
    - Activation Functions (ReLU, Sigmoid, Softmax, etc.)
  - Convolutional Neural Networks (CNNs)
    - Discrete Convolutions and Cross-Correlation
    - Pooling, Subsampling, and Receptive Fields
  - Advanced Architectures: ResNets and UNets
    - Skip Connections and Residual Networks
    - Encoder-Decoder Structures
  - Training Dynamics & Optimisation
    - Loss Functions (MSE, Cross-Entropy)
    - Gradient Descent, SGD, and Adam Optimiser
    - Practical Training Considerations: Dropout, Batch Normalisation, Weight Decay, Learning Rate Scheduling
  - The Chain Rule of Calculus & Backpropagation
    - Classical Backpropagation Recursions
    - Generalisation to Implicit Operators: Bilevel, Fixed-Point, and Continuous Limits
  - Direct Supervised Learning (End-to-End) & Its Pitfalls
    - Data Consistency Problem
    - Lipschitz Dilemma and Adversarial Vulnerability
    - Opaque Implicit Bias
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Introduction to the Coding Challenge (Practice)**
  - Problem Statement: Restoring high-quality images from motion blur and noise
  - Software Stack: PyTorch, DeepInverse (`deepinv`)
  - Baseline Implementation: Mathematical reconstruction method (classical inverse problem approach)
  - Competition Details: Groups of 3–4; evaluate on hidden test set (PSNR/SSIM metrics); model size ≤ 100 MB; CPU inference within 20 minutes

## Tuesday: Bilevel Optimisation and Unrolling

- **11:00 – 13:00: Advanced Deep Learning for Inverse Problems (Lecture)**
  - Recap: Inverse Problems & End-to-End Learning
    - The Inverse Problem Formulation ($y^\delta = Ax^\dagger + \eta$)
    - Pitfalls of End-to-End Learning Revisited
    - Classical Methods vs. Deep Learning Trade-offs
  - Null-Space Networks & Data Consistency
    - The Null Space of Forward Operators
    - Orthogonal Decomposition of Images ($\mathbb{R}^n = \mathcal{N}(A) \oplus \mathcal{R}(A^\top)$)
    - Null-Space Architecture: Enforcing Strict Data Consistency
    - Interpretability and Safety Guarantees
  - Variational Methods & Optimisation Algorithms
    - Inverse Problems as Variational (Regularised) Optimisation
    - Classical Regularisation Techniques
    - Iterative Algorithms: ISTA and PDHG
  - Bilevel Optimisation & Sensitivity Analysis
    - Formulating Hyper-Parameter Learning as Nested Optimisation
    - Introduction to Convex and Non-Convex Optimisation
    - Differentiating Through the Lower Level via the Implicit Function Theorem (IFT)
    - Handling Non-Smooth Functions via Huber Smoothing
  - Learning Regularisers with Guarantees
    - NETT (Network Tikhonov Regularisation)
    - ICNNs (Input Convex Neural Networks) for Recovering Stability Guarantees
  - The Unrolling Principle & Architectures
    - Truncating Iterative Algorithms to Fixed-Depth Learnable Networks
    - LISTA: Learned ISTA
    - Learned Primal-Dual (LPD) Networks as Unrolled PDHG
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: ARC Forum and Social (Optional, no scheduled class)**
  - **14:00 – 15:00:** ARC weekly forum
  - **15:00 onwards:** ARC social hour
  - No formal training session scheduled; attendees may join optional events

## Wednesday: Modular Deep Learning and Generative Models

- **11:00 – 13:00: Modular Deep Learning and Generative AI (Lecture)**
  - Modular Deep Learning via Plug-and-Play (PnP)
    - Breaking the Rigidity of End-to-End and Unrolled Networks
    - The Plug-and-Play Heuristic: Replacing Proximal Operators with Pre-Trained Denoisers
    - PnP-HQS and PnP-ADMM Algorithms
    - Convergence Analysis: Fixed-Point Perspective (Non-Expansive and Contractive Denoisers, Banach's Theorem)
  - Defining Losses & The Jacobian Critique
    - Regularisation by Denoising (RED): Learning from Denoiser Implicit Priors
    - Critical Evaluation of Explicitly Defined Loss Functions
    - Jacobian Critique and its Implications
  - Deep Generative Modelling Frameworks
    - Autoencoders and Variational Autoencoders (VAEs)
      - Encoder–Decoder Structure and the Reparameterisation Trick
      - ELBO (Evidence Lower Bound) Objective
      - VAEs as Learned Latent-Space Priors
    - Generative Adversarial Networks (GANs) and Normalising Flows
  - Score-Based Models and Diffusion
    - From Denoisers to Probability Distributions: Tweedie's Formula
    - Denoising Score Matching
    - The Forward Diffusion Process and Reverse-Time SDE
    - Diffusion Models as Learned Priors for Inverse Problems
    - Langevin Dynamics and Sampling
    - Diffusion Posterior Sampling (DPS) for Solving Inverse Problems
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Coding Challenge (continued)**
  - Continue working in groups on your coding challenge contributions.

## Thursday: Continuous Depth and Implicit Deep Learning

- **11:00 – 13:00: Continuous Depth and Implicit Deep Learning (Lecture)**
  - Deep Learning as Continuous Dynamical Systems
    - ResNets as Forward Euler Discretisations of ODEs
    - Gradient Flow as Continuous Optimisation
    - Neural ODEs and Adaptive Computation
  - Discretisation and Architectural Design
    - From Continuous ODEs to Discrete Network Layers
    - Symplectic Discretisations for Energy-Stable Networks
    - Variational Networks (VNs): Incorporating Physics Through Discretisation Schemes
  - The Early Stopping Paradox & Dynamic Depth
    - Why Fixed Depth Leads to Suboptimality
    - Learning Depth as a Continuous Parameter
    - Resolving the Paradox: Adaptive Network Width and Depth
  - Implicit Deep Learning & Deep Equilibrium Models (DEQ)
    - Fixed-Point Problems and Implicit Function Theorem
    - DEQ Architecture: Single Fixed-Point Condition vs. Finite Layers
    - Memory-Efficient Training via Implicit Differentiation
    - Adjoint Equations for Implicit Backpropagation
  - Connection to Bilevel Learning
    - DEQs as Optimisation-Defined Layers (Bilevel Framework)
    - Implicit Differentiation for Hyperparameter Sensitivity
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Guest Lecture and Q&A**
  - Speaker: [Dr Jonas Latz](https://latzplacian.org), University of Manchester.
  - Topic: Stochastic gradient methods in continuous time for machine learning, including stochastic gradient processes, convergence and ergodicity, and implications for modern ML optimisation practice.
  - Q&A with the guest speaker.

## Friday: Group Presentations

- **10:00 – 12:30: Presentations**
  - Student groups present their solution to the coding challenge.
  - Focus on: Architecture choice, training strategy, and evaluation of results (PSNR/SSIM).
- **12:30 – 13:30: Lunch**
- **13:30: End of Training Week**
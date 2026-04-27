# Schedule

## Monday: Foundations of Deep Learning

- **11:00 – 13:00: Introduction to Deep Learning (Lecture)**
  - Neural Network Architectures: From the Perceptron to MLPs.
  - Activation functions (ReLU, Sigmoid, Softmax etc.).
  - Convolutional Neural Networks (CNNs): Convolution as a local, weight-sharing linear operator; pooling and receptive fields
  - ResNets and skip connections, UNets.
  - Training Dynamics: Loss functions (MSE, Cross-Entropy), Gradient Descent, SGD and Adam. Practical training considerations: dropout, batch normalisation, weight decay, and learning rate scheduling.
  - The Chain Rule of Calculus: Mathematical derivation of Backpropagation.
  - Generalisation of Backpropagation to operators stemming from optimisation problems, fixed-point problems, or continuous limits of network architectures.
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Introduction to the Coding Challenge (Practice)**
  - Problem Statement: Recovering a sharp image from noisy, degraded measurements using a known forward operator.
  - Software Stack: PyTorch, DeepInverse.
  - Baseline Implementation: A total-variation based reconstruction method.
  - Competition: You will compete with your peers in groups of two/three to achieve the highest PSNR and SSIM on a hidden test set. Model weights ≤ 100 MB, inference on CPU within 20 minutes.

## Tuesday: Bilevel Optimisation and Unrolling

- **11:00 – 13:00: Bilevel Optimisation & Unrolling (Lecture)**
  - Bilevel Optimisation: Formulating hyper-parameter learning as a nested upper/lower-level problem.
  - A brief inntroduction to convex and non-convex optimisation and algorithms
  - Differentiating Through the Lower Level: The Implicit Function Theorem (IFT) and sensitivity analysis; handling non-smooth functions via smoothing (Huber loss).
  - The Unrolling Principle: Truncating iterative algorithms to a fixed number of layers with learnable weights trained end-to-end.
  - Unrolled Architectures: LISTA for sparse coding; Learned Primal-Dual (LPD) network as an unrolled PDHG.
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Coding Challenge (continued)**
  - Learning the regularisation parameter of a variational deblurring model via bilevel optimisation, differentiating through the lower-level reconstruction, or using unrolled architectures via Deep Inverse.

## Wednesday: Plug-and-Play Priors

- **11:00 – 13:00: Plug-and-Play Methods (Lecture)**
  - The Plug-and-Play Heuristic: Replacing the proximal operator with a pre-trained denoiser (BM3D, DnCNN, DRUNet); PnP-HQS and PnP-ADMM algorithms.
  - Convergence Analysis: Fixed-point perspective (non-expansive and contractive denoisers, Banach's theorem); optimisation perspective.
  - Regularisation by Denoising (RED).
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Coding Challenge (continued)**
  - Plugging a pre-trained denoiser into a PnP method as a drop-in regulariser for the deblurring problem, and comparing results to the unrolled network.

## Thursday: Generative Models and Implicit Architectures

- **11:00 – 13:00: Generative Models, Continuous Dynamics, and Deep Equilibrium Models (Lecture)**
  - Autoencoders and Variational Autoencoders (VAEs): Encoder–decoder structure; the reparameterisation trick; the ELBO objective; VAEs as learned latent-space priors.
  - Score-Based and Diffusion Models: Denoising score matching; the forward diffusion process and reverse-time SDE; diffusion models as priors for inverse problems.
  - Deep Learning as Dynamical Systems: ResNets as forward Euler discretisations of an ODE; training as an optimal control problem and the adjoint state equation.
  - Deep Equilibrium Models (DEQ): Replacing finite depth with a single fixed-point condition; memory-efficient training via implicit differentiation.
- **13:00 – 14:00: Lunch**
- **14:00 – 16:00: Guest Lecture and Q&A**
  - Topic: Real-world deployment of deep learning in Medical Imaging.
  - Q&A session with guest speaker

## Friday: Group Presentations

- **10:00 – 12:00: Presentations (Session 1)**
  - Student groups present their solution to the coding challenge.
  - Focus on: Architecture choice, training strategy, and evaluation of results (PSNR/SSIM).
- **12:00 – 13:00: Lunch**
- **13:00 – 15:00: Presentations (Session 2)**
  - Continuation of presentations.

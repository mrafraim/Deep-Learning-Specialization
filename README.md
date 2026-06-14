# **Deep Learning N-Days Daily Roadmap**


## **Phase 1: Foundations (Day 1–8)**

| Day | Topic                     | Goal                                                                                                     |
| --- | ------------------------- | -------------------------------------------------------------------------------------------------------- |
| 1   | What is Deep Learning?    | Introduction, history, real-world examples, first neuron intuition, forward propagation of single neuron |
| 2   | Neurons, Weights, Bias & Activations    | Deep dive into neuron structure, weights, bias, activation functions, visualizations       |
| 3   | Forward Propagation       | Manual calculations, numpy implementation, ReLU, Sigmoid, Tanh                                           |
| 4   | Tiny Neural Network       | Build 2-layer network from scratch in numpy                                                              |
| 5   | Loss Functions            | MSE, Cross-Entropy, small examples                                                                       |
| 6   | Optimizers                | Gradient Descent intuition, learning rate, update rules, simple code                                     |
| 7   | Mini Exercise             | Manual neuron calculations, small network experiments                                                    |
| 8   | Phase Summary | wrap-up, code + visuals                                             |


## **Phase 2: First Neural Networks & Backpropagation (Day 9–19)**

| Day | Topic                           | Goal                                    |
| --- | ------------------------------- | -------------------------------------------------------- |
| 9   | Gradient & Derivative Intuition | Calculus review, small examples                          |
| 10  | Backpropagation Basics          | Manual chain rule calculations                           |
| 11  | Backpropagation in Numpy        | Tiny network training step-by-step                       |
| 12  | Full Forward + Backprop Example | Numpy mini training loop                                 |
| 13  | PyTorch Introduction            | Tensors, basic operations, GPU usage                     |
| 14  | PyTorch Neural Network          | Build first simple model                                 |
| 15  | Training loop in PyTorch        | Forward + loss + backward + optimizer step               |
| 16  | Overfitting vs Underfitting     | Visualize loss curves, concept explanation               |
| 17  | Validation & Test split         | Data handling in PyTorch, metrics                        |
| 18  | Hyperparameters                 | Learning rate, epochs, batch size, grid search intuition |
| 19  | Phase Summary                   | Notebook wrap-up, code + visuals                         |


## **Phase 3: Convolutional & Recurrent Networks (Day 20–33)**

| Day | Topic                       | Goal                            |
| --- | --------------------------- | ------------------------------------------------- |
| 20  | CNN introduction               | Filters, stride, padding, convolution example     |
| 21  | CNN Layers                  | Pooling, flatten, fully connected layers          |
| 22  | CNN in PyTorch              | Build simple CNN for MNIST                        |
| 23  | CNN training                | Forward + backward + optimizer, visualize filters |
| 24  | RNN introduction               | Sequence data, hidden state, unrolling            |
| 25  | LSTM & GRU                  | Why LSTM > RNN, gates explanation                 |
| 26  | Simple RNN in PyTorch       | Manual sequence prediction                        |
| 27  | LSTM example                | Text sequence prediction                          |
| 28  | NLP preprocessing           | Tokenization, embedding, padding                  |
| 29  | RNN mini project            | Predict sentiment on small dataset                |
| 30  | CNN + RNN comparison        | When to use which, pros/cons                      |
| 31  | Regularization in CNN/RNN   | Dropout, batch norm, visualization                |
| 32  | Hyperparameters for CNN/RNN | Learning rate, optimizer tuning                   |
| 33  | Phase Summary               | Notebook wrap-up with multiple small examples     |


## **Phase 4: CNN Advanced Mastery (Day 34–44)**

| Day | Focus                              | Goal                                                                       |
| --- | ---------------------------------- | -------------------------------------------------------------------------- |
| 34  | CNN Regularization                 | Dropout placement, BatchNorm behavior (train vs eval), overfitting control |
| 35  | CNN Weight Initialization          | Xavier vs He, dead ReLU problem, empirical comparisons                     |
| 36  | CNN Optimizers                     | SGD vs Adam vs AdamW vs RMSProp, convergence tradeoffs                     |
| 37  | CNN Learning Rate Scheduling       | StepLR, ReduceLROnPlateau, CosineAnnealing, LR intuition                   |
| 38  | CNN Data Augmentation              | Geometric & color transforms, over/under-augmentation risks                |
| 39  | CNN Multi-Class Classification     | Softmax, CrossEntropy, class imbalance, top-k accuracy                     |
| 40  | CNN Multi-Label Classification     | BCEWithLogits, threshold tuning, PR tradeoffs                              |
| 41  | CNN Evaluation & Debugging         | Confusion matrix, ROC/PR curves, error analysis                            |
| 42  | CNN Early Stopping & Checkpointing | Validation-driven stopping, best-model saving                              |
| 43  | CNN Hyperparameter Tuning          | Batch size–LR coupling, weight decay, controlled experiments               |
| 44  | CNN Advanced Mini Project          | Apply all CNN techniques end-to-end (no shortcuts)                         |

## **Phase 5: MLOps / Deployment / Scaling (Day 45–54)**

| Day    | Topic                        | Goal                                                                                    |
| ------ | ---------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| **45** | Intro to Model Deployment    | Understand research vs production, what “serving a model” means, and full pipeline (train → save → serve → predict) |
| **46** | Saving & Loading Models      | Use `torch.save` / `torch.load`, save best CNN weights, load in separate script, verify correctness                 |
| **47** | Inference Pipeline           | Build strict function: image → preprocessing → model → prediction (no training code allowed)                        |
| **48** | FastAPI Basics               | Learn routes, request/response cycle, use `/docs` UI for testing endpoints                                          |
| **49** | CNN + FastAPI Integration    | Wrap inference pipeline into `/predict` endpoint, test with real image upload                                       |
| **50** | Pydantic & Error Handling    | Validate inputs (image only), handle bad inputs cleanly, return proper JSON responses                               |
| **51** | Docker Basics                | Learn containers, write Dockerfile, build image, run container locally                                              |
| **52** | Production Containerization  | Add FastAPI + model into Docker, run with Uvicorn (production-style server)                                         |
| **53** | Stress Testing & Performance | Test multiple inputs, edge cases, batch inference, CPU vs GPU performance                                           |
| **54** | Project Finalization         | Clean code, structure repo, write README, add usage guide & demo outputs                                            |

## **Phase 6: Object Detection Mastery (Day 55–66)**

| Day    | Topic                                | Goal                                                                                                        |
| ------ | ------------------------------------ | ----------------------------------------------------------------------------------------------------------- |
| 55 | Detection Fundamentals               | Understand classification vs detection, bounding boxes, IoU, NMS, mAP metric                                |
| 56 | Dataset Selection & Preparation      | Choose dataset (COCO subset / Pascal VOC / custom), organize images & annotations, train/test split         |
| 57 | CNN Backbone Review                  | Review your CNN knowledge, understand feature maps, anchors, and why CNNs are backbone of detectors         |
| 58 | Pretrained Detection Models          | Explore YOLOv5 / YOLOv8 inference on sample images, visualize predictions, understand confidence thresholds |
| 59 | Fine-tuning Detection Model          | Load pretrained model, fine-tune on small custom dataset                |
| 60 | Advanced Training Tricks             | Use augmentation (flips, scale, color), early stopping, learning rate scheduling for detection              |
| 61 | Evaluation & Metrics                 | Compute mAP, IoU; analyze errors, visualize false positives/negatives                                       |
| 62 | Multi-class / Multi-object Scenarios | Handle multiple objects per image, class imbalance, threshold tuning                                        |
| 63 | Optimization & Inference             | Batch inference, GPU utilization, speed-memory tradeoffs, confidence calibration                            |
| 64 | Detection Project                    | Build a mini project: custom dataset, trained model, evaluation, visualizations                             |
| 65 | Deployment                           | Wrap detection model in a simple FastAPI endpoint locally, allow image upload → detection output            |
| 66 | Portfolio Polish                     | Prepare notebook for portfolio: clean code, explanations, results, plots                                    |

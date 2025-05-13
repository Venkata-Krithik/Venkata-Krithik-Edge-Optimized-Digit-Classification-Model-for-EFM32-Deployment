# Edge-Optimized-Digit-Classification-Model-for-EFM32-Deployment


This project demonstrates a complete pipeline for deploying a deep learning model on a memory-constrained embedded device using **Edge AI techniques** such as **structured pruning**, **quantization**, and **MATLAB-to-C conversion**. The project is implemented and simulated using MATLAB, and targets deployment on microcontrollers like the EFM32 or similar ARM Cortex-M architectures.

---



## 🎯 Objective

To enable real-time digit classification on ultra-low-power microcontrollers by optimizing a neural network model for size, speed, and accuracy using Edge AI techniques.

---

## 🔧 Key Techniques Used

- ✅ **Model Pruning**: Reduces the number of channels/neurons in the network to save memory and computation.
- ✅ **8-bit Quantization**: Converts weights and activations to fixed-point 8-bit format for efficient embedded deployment.
- ✅ **MATLAB-to-C Workflow**: Uses MATLAB Coder or manual export to prepare inference code for microcontrollers.
- ✅ **Memory Profiling**: Compares RAM/Flash usage before and after optimizations.

---

## 📉 Performance Summary

| Metric                   | Baseline Model | Optimized Model |
|--------------------------|----------------|------------------|
| Accuracy                 | ~93%           | ~90%             |
| Flash Usage              | 100%           | 59% (↓ 41%)      |
| RAM Usage                | 100%           | 47% (↓ 53%)      |
| Inference Time           | Real-time      | Real-time        |

---

## 🧪 Implementation Environment

- MATLAB 2023a or later
- Deep Learning Toolbox
- Embedded Coder (optional, for C code generation)

---

## 📝 How to Run

1. Open `FinalEdgeAi.mlx` in MATLAB.
2. Run each section step-by-step to:
   - Load and preprocess data
   - Train base CNN model
   - Apply structured pruning
   - Quantize weights/activations
   - Evaluate accuracy and memory usage
3. Use Embedded Coder to convert the model to C (optional).

---

## 📄 Report

Refer to [`EdgeAi.pdf`](Edge AI/EdgeAi.pdf) for a detailed explanation of:

- Dataset used
- Model architecture
- Optimization pipeline
- Deployment considerations
- Performance benchmarks

---

## 📌 Applications

- Digit recognition on IoT sensors
- Battery-powered edge devices
- Real-time ML inference on microcontrollers
- Embedded systems for classification tasks

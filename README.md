# CIFAR-10 Custom CNN

Custom Convolutional Neural Network built from scratch for CIFAR-10 image classification.  
**Accuracy: 72.46%** | PyTorch | Feature Visualization | Regularization Comparison

*CSC3831 Computer Vision coursework - Newcastle University (Dec 2025)*

---

## Highlights

- **Custom architecture** from scratch: 3 conv layers (32→64→128 filters) + 3 FC layers
- **72.46% test accuracy** on 10-class classification
- **Regularization comparison:** L2, Dropout (p=0.5), Batch Normalization
- **Feature visualization:** Hierarchical learning (edges → textures → abstract)
- **Early stopping:** Best validation at epoch 8, training stopped at epoch 11

---

## Results

| Metric | Value |
|--------|-------|
| Test Accuracy | 72.46% |
| Best Epoch | 8 |
| Total Epochs | 11 |
| Best Regularization | Dropout (p=0.5) |

### Architecture

### Architecture

```
Input: 32x32x3 RGB images
↓
Conv1: 32 filters (3x3) → ReLU → MaxPool
Conv2: 64 filters (3x3) → ReLU → MaxPool
Conv3: 128 filters (3x3) → ReLU → MaxPool
↓
Flatten
↓
FC1: 2048 units → ReLU
FC2: 512 units → ReLU
FC3: 128 units → ReLU
↓
Output: 10 classes (Softmax)
```

---

## Technologies

- **PyTorch** - Deep learning framework
- **CIFAR-10** - 60,000 32x32 color images, 10 classes
- **Adam optimizer** - Learning rate: 0.001
- **Regularization** - Dropout, L2, Batch Normalization

---

## Files

- **Notebooks:** Training, evaluation, feature visualization
- **Report:** Full project documentation

---

## Quick Start

```bash
# Install dependencies
pip install torch torchvision matplotlib

# Dataset downloads automatically via torchvision.datasets.CIFAR10
```

---

## Key Learnings

1. **Dropout outperformed** L2 and Batch Normalization for this architecture
2. **Early stopping prevented overfitting** - performance peaked early
3. **Feature visualization** revealed hierarchical learning from edges to complex patterns
4. **Progressive filter increase** (32→64→128) improved feature extraction

---

## Author

**Kalyani Panambalom**  
Computer Science @ Newcastle University  
Incoming MSc AI @ University of Bristol (Sept 2026)

[LinkedIn](https://linkedin.com//in/kalyani-panambalom-0b2931352)

---

*Last updated: December 2025*


# Hybrid ConvNeXt–Swin Transformer model for AI Image Detection
This repository implements a hybrid deep learning framework designed to detect AI-generated images. The model focuses on identifying subtle structural and textural artifacts that distinguish synthetic content from authentic human-created images.

## Key Technical Highlights
Hybrid Architecture: Combines ConvNeXt (CNN) for local spatial features and Swin Transformer for global contextual dependencies.

4-Channel Input: Processes RGB + Grayscale simultaneously to better capture luminance-based inconsistencies and frequency artifacts.

Adaptive Fusion: Uses an Attention-based module to dynamically weight features from both backbones for more robust classification.

## Model Workflow
Preprocessing: Augmentation and conversion to a 4-channel (RGB-G) tensor.

Feature Extraction: Parallel processing through ConvNeXt-Tiny and Swin-Tiny.

Fusion: Weighted feature integration via an attention mechanism.

Classification: Binary prediction (AI vs. Human) via a fully connected head.

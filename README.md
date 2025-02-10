# Enhanced 3D Content Generation Using Gaussian Splatting and CLIP-Guided Refinement

## Overview

This project explores improving 3D content generation by integrating a CLIP-guided classifier within the Gaussian Splatting framework. The primary goal is to enhance model refinement by addressing limitations in fine geometric details and visual control. While Gaussian Splatting offers efficient 3D scene representation, it struggles with rendering high-quality textures and handling model flexibility. By incorporating a classifier, this work aims to provide guided improvements in the generation process.

## Features

- **Gaussian Splatting for Efficient 3D Representation**
- **CLIP-Guided Refinement** for enhanced geometric accuracy
- **Classifier-Guided Zero-Shot Optimization**
- **Texture Enhancement via UV-Space Refinement**
- **Efficient Mesh Extraction & Optimization**

## Installation

### Prerequisites

Ensure you have the following dependencies installed:

- Python 3.8+
- PyTorch
- CLIP (OpenAI)
- Gaussian Splatting Renderer
- NVIDIA GPU with CUDA support (Recommended)

```bash
pip install torch torchvision
pip install clip-by-openai
pip install numpy matplotlib
```

## Usage

### Training the Model

```bash
python train.py --dataset path/to/images --epochs 500
```

### Rendering a 3D Model

```bash
python render.py --input path/to/image.png --output path/to/output.obj
```

## Results

The enhanced method showed some improvements in target feature refinement but faced challenges with rendering flexibility and classifier influence.

| Model   | Standard Rendering | CLIP-Guided Refinement |
| ------- | ------------------ | ---------------------- |
| Model A | ✅                  | ✅ (Minor improvements) |
| Model B | ✅                  | ❌ (Limited impact)     |

## Future Work

- **Adaptive Learning Rates** for classifier-model interactions
- **Feature-Specific Loss Functions** for targeted improvements
- **Alternative Classifier Architectures**
- **Real-Time Processing Enhancements**

## Citation

If you use this work, please cite:

```bibtex
@article{zhang2025enhanced3d,
  author = {Hongyang Zhang},
  title = {Enhanced 3D Content Generation Using Gaussian Splatting and CLIP-Guided Refinement},
  year = {2025},
  institution = {The University of Auckland}
}
```

## Contact

For questions, please contact [hzha464@aucklanduni.ac.nz](mailto\:hzha464@aucklanduni.ac.nz).


# A Convolutional Neural Network Ensemble Model for Pneumonia Detection

## Project Overview

This repository contains our implementation and extension of the research paper **"A Convolutional Neural Network Ensemble Model for Pneumonia Detection"**. Our project was completed in two phases:

1. **Phase 1**: Reproduction of the original paper's methodology and results from scratch
2. **Phase 2**: Enhancement of the original model with attention mechanisms and dynamic threshold optimization

## Team Members

- Sahal Saeed
- Fardeen Farhat
- Zain Ul Wahab

## Original Research Paper Implementation (Phase 1)

In Phase 1, we faithfully reproduced the methodology proposed in the original research paper:

### Architecture Details

- Base CNN architecture with 3 convolutional layers
- Three separate models trained with different kernel sizes:
  - Model 1: 3×3 kernels
  - Model 2: 5×5 kernels
  - Model 3: 7×7 kernels
- Final ensemble model combining predictions from all three models

### Implementation Steps

1. Dataset preparation and preprocessing
2. Implementation of the CNN architecture with configurable kernel sizes
3. Training of three separate models (3×3, 5×5, 7×7)
4. Development of the ensemble mechanism to combine model outputs
5. Evaluation and validation against the original paper's results

## Enhanced Model with Attention Mechanism (Phase 2)

For Phase 2, we made significant contributions to improve the original paper's approach:

### Key Contributions

1. **Attention Mechanism**: We integrated an attention mechanism after the third convolutional layer to:
   - Enhance the model's focus on fine-grained details in chest X-ray images
   - Enable the model to better differentiate between healthy and pneumonia-affected regions
   - Reduce class bias and mitigate overfitting issues

2. **Dynamic Threshold Optimization**: We developed a method to dynamically determine optimal thresholds for the sigmoid function at the output layer:
   - Replaced hard-coded threshold values with dynamically computed ones
   - Implemented adaptive threshold optimization based on validation data
   - Improved classification performance across different test scenarios

### Extended Implementation Details

1. Attention mechanism design and integration
2. Threshold optimization algorithm development
3. Training of all three kernel-specific models with the enhanced architecture
4. Ensemble model implementation with the attention-enhanced base models
5. Comprehensive evaluation and comparative analysis

## How to Use This Repository

This repository contains the implementation code for both Phase 1 (original paper reproduction) and Phase 2 (enhanced model with attention mechanism). The research paper documenting our methodology and findings is available in both PDF and DOCX formats.

Key files include:
- Implementation code for the original CNN models with different kernel sizes
- Dynamic threshold optimization algorithms
- Training and evaluation scripts
- Both phases files which included the above features are included in the repository.


## Research Paper

Our implementation and findings are documented in detail in the accompanying research paper, which follows the IEEE format. The paper includes comprehensive evaluation metrics and comparative analysis between the original and our enhanced models.

The research paper is available in both PDF and DOCX formats in this repository.

## Acknowledgments

We acknowledge the authors of the original research paper "A Convolutional Neural Network Ensemble Model for Pneumonia Detection" for their foundational work that inspired this project.

Checkout the research paper at [A Convolutional Neural Network Ensemble Model for Pneumonia Detection](https://www.sciencedirect.com/science/article/pii/S2772442523000436)

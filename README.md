# Deep-Learning-Application-in-Data-Science

## Handwritten Digit Classification Using PyTorch

### Project Overview

This project implements a Multilayer Perceptron (MLP) neural network using PyTorch to classify handwritten digits from 0 to 9. It uses the Scikit-learn Digits dataset, which contains 8 × 8 grayscale images represented by 64 numerical pixel features.

### Objectives

- Explore and prepare a publicly available image dataset.
- Design and train a neural network for multiclass classification.
- Monitor training and validation loss.
- Evaluate model performance using multiple classification metrics.
- Analyze misclassified examples, limitations, and potential improvements.

### Dataset

The project uses the built-in Scikit-learn Digits dataset.

- **Samples:** 1,797
- **Input features:** 64 pixel values per image
- **Classes:** 10 digit classes (0–9)
- **Image dimensions:** 8 × 8 pixels

Pixel values are normalized to the range [0, 1]. Stratified training, validation, and test splits are used to maintain class proportions.

### Model Architecture

The PyTorch MLP contains:

- Input layer: 64 features
- Hidden layer 1: 128 neurons with ReLU activation
- Hidden layer 2: 64 neurons with ReLU activation
- Dropout regularization
- Output layer: 10 class scores

The model is trained using the Adam optimizer and cross-entropy loss.

### Recorded Results

The recorded experiment achieved:

| Metric | Result |
|---|---:|
| Test accuracy | 97.78% |
| Macro precision | 0.9782 |
| Macro recall | 0.9776 |
| Macro F1-score | 0.9777 |
| Correct test predictions | 352 / 360 |

These values describe the recorded run and may vary if the experiment is rerun with different settings or randomness.

### Visualizations and Outputs

The project generates visualizations and evaluation files, including:

- Example images from the Digits dataset
- Training and validation loss curves
- Test confusion matrix
- Per-class recall chart
- Examples of misclassified test images
- Test metrics and classification report
- Prediction results and experiment summary

Generated files are organized in the `outputs/` directory.

### Project Files

- `Week 5 Task Deep Learning Application in Data Science.ipynb` — notebook containing the implementation and evaluation.
- `Week 5 Task Deep Learning Application in Data Science.docx` — detailed project report.
- `outputs/` — generated figures, metrics, predictions, and experiment artifacts.
- `README.md` — project overview and execution instructions.

### Installation

Install the required Python libraries in your environment:

```bash
pip install numpy pandas matplotlib scikit-learn torch
```

### How to Run

1. Download or clone this repository.
2. Install the required dependencies.
3. Open the Jupyter notebook.
4. Run the notebook cells in order.
5. Inspect the generated results in the `outputs/` directory.

If PyTorch is not installed, install it for your operating system and Python environment using the official PyTorch installation instructions.

### Limitations and Future Improvements

The dataset uses small 8 × 8 images, which limits the visual detail available to the model. Some handwritten digits have similar pixel patterns and may be confused. Future work could compare the MLP with a convolutional neural network, conduct systematic hyperparameter tuning, and repeat evaluation across multiple random seeds.


### Report

The accompanying Word report provides the detailed methodology, architecture rationale, evaluation analysis, visualizations, limitations, and conclusions.

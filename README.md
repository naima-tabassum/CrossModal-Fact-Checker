# CrossModal-Fact-Checker

A multimodal deep learning project for detecting out-of-context misinformation by checking whether an image semantically matches its accompanying text or claim.

## Project Overview

The system analyzes an image and a textual claim together.

- The image branch extracts visual features.
- The text branch uses BERT to extract textual features.
- Image and text representations are projected into a shared embedding space.
- Cosine similarity and a fusion classifier are used to determine whether the image-text pair is matched or mismatched.

A mismatched image-text pair is treated as out-of-context misinformation.

## Main Technologies

- Python
- PyTorch
- BERT
- CLIP / Visual Feature Extraction
- Hugging Face Transformers
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Gradio
- Google Colab

## Datasets

The project uses data derived from:

- COCO 2017
- Flickr30k
- NewsCLIPpings
- CIFAKE

Large dataset files are not included in this repository. The notebook contains the required data preparation and download steps.

## Repository Files

- `FinalNotebook.ipynb` — Complete implementation, preprocessing, training, evaluation, and demo.
- `FinalReport.pdf` — Final project report.

## How to Run

1. Open `FinalNotebook.ipynb` in Google Colab.
2. Select a GPU runtime.
3. Mount Google Drive.
4. Install the required libraries.
5. Configure Kaggle credentials locally for CIFAKE.
6. Run the dataset preparation cells.
7. Create the balanced manifest.
8. Run preprocessing.
9. Define the multimodal model.
10. Run the training pipeline.
11. Run evaluation and visualization cells.
12. Run the Gradio demo.

## Important Note

The `kaggle.json` credential file is not included in this repository. Users must configure their own Kaggle API credentials.

## Project Scope

The current implementation mainly focuses on detecting whether an image and its accompanying text are semantically matched or mismatched.

Future extensions can include separate image authenticity and text authenticity detection.

## Authors

- Wasikul Hasan Fahim
- Md. Akif Hossain
- Naima Tabassum Antora

Department of Computer Science and Engineering  
University of Asia Pacific  
Dhaka, Bangladesh

# Health Sound Analysis Using Mel Spectrograms

This project, developed by myself [Abu Ubaida Aljerah](https://github.com/Ubaida10) and [Tahir Mustafvi](https://github.com/M-TahirMustafvi), uses machine learning and audio processing techniques to analyze heart and lung sounds, aiding in the detection of potential health issues. By converting sound recordings into Mel spectrograms and using a neural network model trained on specific medical conditions, this project identifies patterns associated with various diseases, providing a non-invasive approach to preliminary health diagnostics.

## Table of Contents
- [Overview](#overview)
- [Project Objective](#project-objective)
- [Features](#features)
- [Dataset](#dataset)
- [Setup and Requirements](#setup-and-requirements)
- [Installation](#installation)
- [Usage](#usage)
- [How It Works](#how-it-works)
- [Model Architecture](#model-architecture)
- [Results And Evaluation](#results-and-evaluation)
- [Acknowledgments](#acknowledgments)


## Overview

The **Health Sound Analysis Using Mel Spectrograms** project processes heart and lung audio recordings and classifies them to detect potential health issues. The model was trained on a labeled dataset that includes audio samples of different diseases, enabling it to recognize specific sound patterns associated with each condition.

## Project Objective

This project aims to:
- Enable early detection of heart and lung diseases through sound analysis.
- Provide a preliminary diagnostic tool for health professionals and researchers.
- Explore the potential of Mel spectrograms in medical applications.

## Features

- **Heart and Lung Sound Analysis**: Processes and classifies heart and lung sounds, distinguishing between healthy and diseased conditions.
- **Disease Classification**: Uses machine learning to identify diseases based on sound patterns from a labeled dataset.
- **User-Friendly Output**: Provides insights on detected health issues for preliminary analysis.
- **Machine Learning Integration**: Implements a deep learning model for high-accuracy classification of health sounds.

## Dataset

The dataset used in this project contains heart and lung audio recordings, each labeled with a specific disease condition. The data is openly available, and the link can be accessed here: [Dataset Link](https://www.kaggle.com/datasets/vbookshelf/respiratory-sound-database?resource=download). This dataset includes:
- **Heart Sound Samples**: Normal and abnormal heartbeats, murmurs, etc.
- **Lung Sound Samples**: Normal breathing sounds and abnormal sounds (e.g., wheezes, crackles) indicating respiratory conditions.

## Setup and Requirements

### Prerequisites

- **Python 3.7** or higher
- Libraries:
  - `librosa` - for audio processing and spectrogram generation
  - `numpy` - for numerical computations
  - `pandas` - for data manipulation
  - `tensorflow` - for building and training the neural network model
  - `scikit-learn` - for evaluation metrics
  - `matplotlib` and `seaborn` - for visualization

## Installation

Install the required dependencies:

```bash
pip install librosa numpy pandas tensorflow scikit-learn matplotlib seaborn
```


## Usage

- Step 1: Data Loading
Load and inspect the dataset to familiarize yourself with the structure and labels.


- Step 2: Convert Audio to Mel Spectrograms
Use `librosa` to process audio files and generate Mel spectrograms.

- Step 3: Train the Model
Define the neural network model, train it on the spectrogram data, and evaluate its accuracy.


- Step 4: Evaluate and Interpret Results
After training, evaluate the model’s performance using test data and view the classification report for insights.

For more details look at the provided Jupyter Notebook

## How It Works

- Sound Capture: Audio files are loaded and converted to Mel spectrograms, which represent sound frequencies over time.
- Spectrogram Processing: Mel spectrograms highlight frequency patterns related to specific health conditions.
- Model Training: A convolutional neural network (CNN) is trained on labeled spectrograms, learning to differentiate normal and diseased sounds.
- Prediction and Classification: The trained model classifies new audio inputs and predicts associated diseases.

## Model Architecture

The model leverages a Convolutional Neural Network (CNN) architecture, ideal for identifying patterns in Mel spectrogram images. Layers include:

- Convolutional Layers: Capture important features in the spectrograms.
- Pooling Layers: Reduce dimensionality, retaining essential information.
- Dropout Layers: Mitigate overfitting.
- Fully Connected Layer: Maps extracted features to disease classifications.

![image](https://github.com/user-attachments/assets/484383ca-8867-4c0b-8fa2-1f12d46aab0d)


## Results and Evaluation

Model performance is assessed using metrics such as accuracy, precision, and recall, alongside visualization with confusion matrices and ROC curves for detailed analysis.

![image](https://github.com/user-attachments/assets/ff280fa7-e750-47fd-81fe-b0a6ad3c514c)


## Acknowledgments

We acknowledge the open dataset providers and the developers of libraries such as `librosa` and `tensorflow`, whose resources have greatly facilitated this project.

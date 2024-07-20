# Vehicle-Classification
AI-based Vehicle Classification system using machine learning to identify and classify cars, bikes, and rickshaws from images.

## Table of Contents
- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Proposed Solution](#proposed-solution)
- [Data Collection and Manipulation](#data-collection-and-manipulation)
  - [Data Collection](#data-collection)
  - [Data Labeling and Augmentation](#data-labeling-and-augmentation)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Future Work](#future-work)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Introduction
In this modern era of technology, the world is quickly adopting Artificial Intelligence. Simple systems are being replaced by AI systems that can evolve with respect to the environment. Our project, Vehicle Identification and Classification, is a prerequisite for an AI-based parking system. This model can distinguish between cars, bikes, and rickshaws in real-time, which is beneficial for automated parking systems.

## Problem Statement
Workers in parking areas around malls, bazaars, markets, and busy areas organize vehicles. This task becomes challenging during rush hours. Our model aims to assist in this environment by classifying vehicles into three categories: Cars, Bikes, and Rickshaws.

## Proposed Solution
Our model can be one of the basic modules of an automated AI parking system, distinguishing between cars, bikes, and rickshaws. 

## Data Collection and Manipulation

### Data Collection
- **Bikes:** More than 100 pictures
- **Cars:** Almost 150 pictures
- **Rickshaws:** 100 pictures

### Data Labeling and Augmentation
We used Roboflow for labeling and augmenting the data. The following techniques were applied:
- Horizontal Flip
- 90° Rotation (Clockwise, Counter-Clockwise, Upside Down)
- Crop (0% Minimum Zoom, 17% Maximum Zoom)
- Random Rotation (Between -20° and +20°)
- Shear (±20° Horizontal, ±20° Vertical)
- Grayscale (Applied to 30% of images)

After augmentation, the dataset increased from 339 images to 1017 images.

## Model Training and Evaluation
The model training and evaluation were performed using various machine learning techniques. The Jupyter notebook file (`Vehicle Classification (CV ASSIGN).ipynb`) contains the complete code and steps for training and evaluating the model.

## Project Structure
The project directory structure is as follows:
```
Vehicle Classification/
│
├── Vehicle Classification (CV ASSIGN).ipynb   # Jupyter notebook with project code
├── _classes.csv   # Trained Model or lebelled data information
├── README.roboflow.txt   # Dataset information from Roboflow
├── README.dataset.txt   # Additional dataset information
├── LICENSE   # License file
```

## Usage
To use the project, follow these steps:
1. Clone the repository:
    ```bash
    git clone https://github.com/usamaGitHub321/Vehicle-Classification.git
    ```
2. Open the Jupyter notebook (`Vehicle Classification (CV ASSIGN).ipynb`) and run the cells to see the model training and evaluation process.

## Future Work
- **Web Interface**: Develop a web interface for the model to allow real-time classification of vehicle images.
- **Model Improvement**: Enhance the model accuracy by experimenting with different architectures and hyperparameters.
- **Data Expansion**: Collect and label more data to improve the model's performance.

## License
This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Acknowledgements
- **Roboflow**: For providing tools for data labeling and augmentation.
- **COMSATS**: For supporting the project and providing resources.

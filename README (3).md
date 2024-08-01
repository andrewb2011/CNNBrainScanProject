
# Brain Tumor Detection




## Authors

- Shayan Akhoondan - []()
- Shahbozbek Hakimov - []()
- Andrew Ballard - [@andrewb2011](https://www.github.com/andrewb2011)
- Krish Naik - []()



## Dataset

The dataset used for this project can be downloaded from [this link](https://drive.google.com/file/d/1zEgzBlTUDzCWpDOSutfyRCcPhbux0rPV/view). 
## Installation

To use the dataset and code in Google Collab:
1. Download the dataset from the link above
2. Open the code in a Google Collab environment
3. Drag the zip file in the file directory on the left side of Google Collab
4. Wait a few minutes for the folder to upload. There should be a circle progress bar at the bottom of the file directory
5. Once the file is uploaded. You can run the code blocks as necessary.

   
## Tech Stack

**Language:** Python3

**Development:** Google Collab

**Libraries:** Tensorflow, Numbpy, MatPlotLib


## Project Overview

### Synopsis of Problem Statement
Medical misdiagnosis and malpractice are increasing concerns, with overworked professionals sometimes making errors. This project aims to provide radiologists with an assistive tool to diagnose brain tumors using a machine learning model trained on real-life MRI image data. This model serves as a reliable second opinion, reducing the risk of human error and ensuring timely and accurate diagnoses.

### Data/Benchmark Description
We utilized two labeled image sets from Kaggle. The primary dataset is split into training (80%) and testing (20%) sets, containing around 6000 and 2000 images respectively, of normal brains and brains with tumors. A secondary dataset, with 3200 images, is used to evaluate the model's performance on unseen data.

### Main Approach/Algorithms Used
We implemented a Convolutional Neural Network (CNN) using the TensorFlow library due to its strong pattern recognition capabilities in image processing tasks. Additional libraries such as NumPy and Matplotlib were used for data manipulation and visualization.

### Result Highlight
Our model achieved high accuracy in detecting brain tumors, demonstrating its potential as a reliable diagnostic tool. The scalability and runtime were optimized to ensure the model could process large datasets efficiently.

### Improvements after the Last Presentation
Based on feedback from the last presentation, we made several improvements:
- Enhanced the CNN architecture for better performance.
- Improved data augmentation techniques to increase the robustness of the model.
- Optimized the model's runtime and scalability.

## Problem Statement and Data/Benchmark Description

### Problem Statement
Misdiagnosis in the medical field can have severe consequences, and overworked doctors are more prone to making errors. A second opinion is often sought, but this can be time-consuming. Our project aims to develop a machine learning model that provides an immediate second opinion on MRI scans, assisting doctors in making accurate diagnoses and reducing the risk of malpractice.

### Data/Benchmark Description
We used two labeled image sets from Kaggle:
1. **Primary Dataset**: Contains approximately 6000 training images and 2000 testing images, split into subfolders for normal brains and brains with tumors. Images are in JPEG format.
2. **Secondary Dataset**: Contains about 3200 images for evaluating the model's performance on unseen data.

The datasets provide a comprehensive benchmark for training and testing the model's accuracy and robustness.

## Approaches, Algorithms, and Programming Tools Used

### Approaches and Algorithms
Our primary approach was to use a Convolutional Neural Network (CNN) due to its efficacy in image pattern recognition. The steps included:
- **Data Preprocessing**: Normalizing and augmenting the MRI images to improve the model's generalization.
- **Model Training**: Using TensorFlow to build and train the CNN on the labeled datasets.
- **Model Evaluation**: Assessing the model's performance on the test set and secondary dataset.

### Programming Tools
- **Python3**: Primary programming language.
- **Google Colab**: Development environment for coding and testing.
- **TensorFlow**: For building and training the CNN.
- **NumPy**: For data manipulation.
- **Matplotlib**: For data visualization and creating accuracy graphs.

### Source Code Structure
The source code is organized as follows:
- **Data Loading and Preprocessing**: Scripts for loading, normalizing, and augmenting the image data.
- **Model Definition and Training**: Scripts for defining the CNN architecture and training the model.
- **Evaluation and Visualization**: Scripts for evaluating the model's performance and visualizing the results.

### System Diagram
```plaintext
+------------------+      +-----------------+      +------------------+
|   MRI Image Data | ---> | Data Preprocessing | ---> |  CNN Training   | 
+------------------+      +-----------------+      +------------------+
                                                                 |
                                                                 v
                                                       +------------------+
                                                       | Model Evaluation |
                                                       +------------------+

# Brain Tumor Detection




## Authors

- Shayan Akhoondan - [@Shayan414](https://www.github.com/Shayan414)
- Shahbozbek Hakimov - [@ShahbozbekH](https://www.github.com/ShahbozbekH)
- Andrew Ballard - [@andrewb2011](https://www.github.com/andrewb2011)
- Krish Naik - [@KrishNaik707](https://www.github.com/KrishNaik707)



## Dataset

The dataset used for this project can be downloaded from [this link](https://drive.google.com/file/d/1zEgzBlTUDzCWpDOSutfyRCcPhbux0rPV/view). 
## Installation

To use the dataset and code in Google Collab:
1. Download the dataset from the link above
2. Open the notebook in a Google Collab environment
3. Drag the zip file in the file directory on the left side of Google Collab
4. Wait a few minutes for the folder to upload. There should be a circle-shaped progress bar at the bottom of the file directory
5. Once the file is uploaded you can run the code blocks as necessary

   
## Tech Stack

**Language:** Python3

**Development:** Google Collab

**Libraries:** Tensorflow, Numbpy, MatPlotLib


## Project Overview

### Synopsis of Problem Statement
Medical misdiagnosis and malpractice are increasing concerns, with overworked professionals sometimes making errors. This project aims to provide radiologists with an assistive tool to diagnose brain tumors using a machine learning model trained on real-life MRI image data. This model serves as a reliable second opinion, reducing the risk of human error and ensuring timely and accurate diagnoses.

### Data/Benchmark Description
We utilized two labeled image sets from Kaggle. The primary dataset is split into training (80%) and testing (20%) sets, containing around 6000 and 2000 images respectively, of normal brains and brains with tumors. A second dataset, with 3200 images, is used to evaluate the model's performance on other data.

### Main Approach/Algorithms Used
We implemented a Convolutional Neural Network (CNN) using the TensorFlow library due to its strong pattern recognition capabilities for processing images. Additional libraries such as NumPy and Matplotlib were used for data manipulation and visualization.

### Result Highlight
Our model achieved high accuracy in detecting brain tumors, demonstrating its potential as a reliable diagnostic tool. The scalability and runtime were optimized to ensure the model could process large datasets better.

### Data/Benchmark Description
We used two labeled image sets from Kaggle:
1. **Primary Dataset**: Contains approximately 6000 training images and 2000 testing images, split into subfolders for normal brains and brains with tumors. Images are in JPEG format.
2. **Secondary Dataset**: Contains about 3200 images for evaluating the model's performance on outside data.

The datasets provide a comprehensive benchmark for training and testing the model's accuracy and robustness.

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
- **Import Libraries and Data**:
- **Model Setup and Data Augmentation**:
- **Model Traning and Validation Results**: 
- **Model Evaluation on Test Dataset w/ Various Trends**: 
- **Model Evaluation on Outside Dataset w/ Various Trends**: 

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

# Breast-Cancer-Detection-Model

Project Title: Early-Stage Breast Cancer Detection using Deep Learning Models

Project Overview:
The incidence of breast cancer has been increasing, emphasizing the need for early detection and intervention. This project focuses on building an AI model using deep learning techniques to predict early-stage breast cancer. By leveraging advanced data analysis and feature extraction methods, the model aims to identify subtle patterns and markers indicative of breast cancer, leading to timely diagnoses and improved treatment outcomes.

Dataset:
The project utilizes a breast cancer dataset obtained from Kaggle. It consists of two CSV files, one containing image file paths and associated descriptions, and the other containing patient details such as ID, breast density, image view, and abnormality type. The dataset also includes a folder with corresponding JPEG images.

Project Workflow:

Importing Libraries and Dataset: Relevant libraries are imported, and the breast cancer dataset is loaded. Initial exploration is performed to gain insights into the dataset.

Data Cleaning: Unnecessary columns are dropped, and missing values are handled using the backward fill (bfill) method. Column names are renamed for convenience.

Image Processing: The breast histopathology images dataset is read from the drive using the glob library. Two separate lists are created to store cancerous and non-cancerous images.

Exploratory Data Analysis (EDA): EDA is conducted using Seaborn library, including count plots, bar graphs, count plots, and pie charts, to gain a deeper understanding of the dataset.

Data Sampling: Due to the large size of the dataset, a random sample of 2000 images is selected for model training to reduce computational complexity.

Data Split: The dataset is divided into training and test sets to evaluate the model's performance accurately.

Model Building: Convolutional Neural Networks (CNNs) are employed to construct the model. Different pre-trained models such as ResNet152, VGG16, and ResNet50 are utilized using transfer learning concepts. The models are trained on the selected dataset, and their accuracies are evaluated.

Model Evaluation: The accuracy of the trained models is assessed using both the training and test datasets. The model with the highest accuracy is selected as the top-performing model.

Conclusion:
This project demonstrates the development of an AI model using deep learning techniques to predict early-stage breast cancer. By training on a diverse and comprehensive dataset, the model can identify subtle patterns and markers that may not be easily detected by human observers. The top-performing model, ResNet50, achieved high accuracy on both the training and test datasets, showcasing its potential as a valuable tool for early-stage breast cancer detection.

This project contributes to the field of medical diagnostics by offering an automated and efficient method for breast cancer detection, enabling timely interventions and improved patient outcomes. Further enhancements can be made by incorporating additional datasets, refining the model architecture, and conducting extensive validation and clinical trials.

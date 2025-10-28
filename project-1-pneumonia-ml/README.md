# Project 1 - Pneumonia Classification in Chest X-rays (Classical Machine Learning)

## Objective
Develop a machine learning model to classify chest X-ray images between pneumonia and normal (No Finding) cases using the NIH ChestX-ray14 dataset.  
The main goal of this project is to understand and apply the basic steps of an ML workflow in medical imaging.

## Dataset
- Source: NIH ChestX-ray14 (The Cancer Imaging Archive)
- Subset used: around 300 balanced images (Pneumonia vs No Finding)
- Resolution: 128x128 grayscale
- Preprocessing: normalization (0–1), flattening, and dimensionality reduction with PCA (95% variance retained)

## Results and discussion
The models achieved AUC values between 0.55 and 0.62, showing limited ability to separate the classes.  
This is mainly due to the small dataset size and the nature of classical ML models, which do not capture spatial structure in images.

In medical imaging, individual pixels have no meaning by themselves.  
Relevant visual patterns (edges, textures, lung regions) require models that analyze spatial relationships, such as convolutional neural networks (CNNs).  
For this reason, classical ML methods are not well suited for direct image analysis.

## Conclusion
This project demonstrates a complete classical ML workflow — preprocessing, training, evaluation, and analysis.  
Although performance is limited, it provides a solid foundation for understanding basic ML concepts and motivates the transition to deep learning approaches for more complex medical imaging tasks.

## Author
Cristian Such Clavel

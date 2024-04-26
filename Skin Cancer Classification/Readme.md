# Introduction

Early detection identified by dermoscopy images significantly decreases the mortality rate from skin cancer. However, the accuracy of the system diagnosis is impacted by multiple factors. A significant issue in this procedure arises during the process of acquiring images. The image quality in medical photography is frequently affected by unanticipated circumstances such as noises and brightness variations, initial digitalization, and sampling. In this work, we suggest a method to reduce the possibility of erroneous diagnosis. The proposed approach begins with preprocessing the data set through CNN and deep learning techniques for data visualization, preprocessing, and augmentation. This preprocessing aids in accelerating the rate of reorganization by eliminating all irrelevant textures. The outcomes identified a 96% accuracy rate with a 4% margin of error. This scheme demonstrated a high degree of accuracy in determining the images, as evidenced by its Precision and F1 Scores of 85% and 87%, respectively.

# Dataset

This dataset is a collection of JPEG files containing either cancerous or non-cancerous skin images. This dataset is perfect for binary classification. Each class, either cancerous or non-cancerous, is split into training and testing sets. 

This dataset was obtained from Kaggle: https://www.kaggle.com/datasets/kylegraupe/skin-cancer-binary-classification-dataset

# Methodology

The methodology for utilizing Convolutional Neural Networks (CNNs) for image classification involves several crucial steps to ensure precision and accuracy. Firstly, data loading and resizing are performed, where raw image data is read and resized to a consistent size, such as (180,180), to meet CNN input requirements. Next, data scaling is conducted to standardize pixel values within the appropriate range by dividing them by 255. Data augmentation follows, employing random transformations to enhance dataset heterogeneity and broaden the model's training capabilities. Subsequently, data processing involves classification into cancerous and non-cancerous categories using CNN, incorporating augmentation to handle image variations. The architecture comprises dropout, convolutional, max-pooling, and dense layers for feature extraction, spatial reduction, and final classification. Training utilizes the Sparse Categorical Cross Entropy loss function and the 'Adam' optimizer, with a 75%-25% training-testing data split to prevent overfitting. Finally, data analysis involves preprocessing images into numpy arrays and separating them into training and testing sets for reliable predictions. This comprehensive methodology ensures the effectiveness of CNN-based image classification for skin cancer detection.

# Conclusion
To expedite accurate skin cancer detection, we developed a method combining CNN and Deep Learning, using dermatoscopic images for training and evaluation. With a 75% training and 25% testing data split, our model achieved 98% accuracy after 40 epochs. Future work aims to refine the model for challenges like class imbalances and varying image qualities, potentially aiding dermatologists and doctors in faster detection processes, including setting up detection camps in vulnerable areas. Additionally, integrating security and verification measures could enhance the model's applicability in medical settings.

# Find the Conference Paper on IEEE Xplore

https://ieeexplore.ieee.org/document/10489085
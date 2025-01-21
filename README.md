# Dog Breed Classification Using ResNet-50

## Overview
This project utilizes advanced deep learning techniques with the ResNet-50 model to classify dog images into their respective breeds, there were 120 unique dog breeds in the Dataset.

## Dataset
The dataset used in this project originates from the Dog Breed Identification competition. It contains 10,222 labeled images of dogs across various breeds, showcasing diverse lighting, poses, and backgrounds.

- **Dataset link**: [Dog Breed Identification](https://www.kaggle.com/competitions/dog-breed-identification)

## Model Details

### Base Model
- **ResNet-50**: The ResNet-50 architecture served as the foundation for this project. Pre-trained weights, available on TensorFlow Hub, were employed to accelerate training and improve accuracy for dog breed classification.
- **Model link**: [ResNet-50 TensorFlow Model](https://www.kaggle.com/models/tensorflow/resnet-50/TensorFlow2/classification/1)

### Training Process
- **Training Images**: The model was initially trained on a subset of 1,000 images and subsequently on the full dataset of 10,222 images.
- **Hardware Used**: Training was conducted on an RTX 4070 Super GPU, enabling efficient computation and reduced training time.
- **Optimizer**: Adam optimizer was used for its adaptability.
- **Loss Function**: Categorical Crossentropy was utilized to handle the multi-class classification task effectively.
- **Metrics**: Accuracy was chosen as the primary metric to evaluate the model's performance.

Additional dense layers were added to the pre-trained ResNet-50 model to fine-tune it to adjust to the 120 different dog breeds to be classified.

### Results
The model achieved the following performance metrics on the validation dataset:
- **Loss**: 0.3249
- **Accuracy**: 90.5%


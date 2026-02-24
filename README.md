# Pretrained-LC2500-
# Lung and Colon Cancer Classification using ResNet-50
I implemented a deep learning project that classified histopatholigical images into 5 classes using a pretrained ResNet50  model trained on the LC25000 dataset.

This project uses Transfer Learning with a Pretrained ResNet50 model to classify lung and colon tissue images. I only retrained the final classification layers to achieve good results without full model training.


# Dataset 
The dataset used was the LC25000 dataset gotten off kaggle, which contains 25000 histopathological images with 5 classes. The original image were 768x768 but was resized to match the ImageNet image size of 224x224. Basic Data Augmentation was used to act as a regularizer to prevent overfitting.

# Model architecture
The model used was a pretrained ResNet50 trained on the ImageNet data. All the layers of the architecture were frozen besides the final classification layer and the final ouput layer was changed to match my dataset task

# Final Results
I used the Accuracy metric to track my results, achieving a Train Accuracy of 95.96% and a Test Accuracy of 96.76%. This close gap indicates that the model generalized well to unseen data.



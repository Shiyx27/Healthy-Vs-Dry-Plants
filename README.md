# Healthy-Vs-Dry-Plants
This project aims to classify images of plants as either healthy or dry using a deep learning approach
Data Preparation:
   The dataset consists of images of healthy plants and dry plants.
   File paths for the images are obtained, and labels are assigned (0 for healthy, 1 for dry).
   The data is shuffled and split into training and validation sets.
Data Augmentation:
   Image data generators are created for both training and validation sets.
   Data augmentation techniques such as rotation, width and height shifting, shear, zoom, and horizontal flipping are applied to the training data to increase its diversity and robustness.
Model Architecture:
   The MobileNetV2 pre-trained model is used as the base model.
   The top layers of the base model are frozen, and custom classification layers are added on top.
   Global average pooling, dense, and sigmoid activation layers are added for classification.
Model Compilation and Training:
   The model is compiled with the Adam optimizer and binary cross-entropy loss function.
   The model is trained on the training data using the fit method, with validation data provided to monitor performance.
   Training is conducted for 15 epochs.
Model Evaluation:
   The trained model is evaluated on the validation set to assess its performance.
   Test accuracy and loss are computed.
Result:
   The model achieves a test accuracy of approximately 85.71%, indicating its effectiveness in distinguishing between healthy and dry plants.

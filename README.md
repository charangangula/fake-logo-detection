# fake-logo-detection
This project implements a Real/Fake Logo detection system using deep learning. The goal is to train a Convolutional Neural Network (CNN) to distinguish between real and fake logos. The dataset consists of images of both genuine and fake logos, and the model is trained to classify these images into their respective categories.

Loading and Preprocessing Images
The script first loads and preprocesses the images from the specified paths. Images are resized to a common size and converted to NumPy arrays. The Inception V3 preprocessing function is applied to the image arrays.

Concatenating Data
Fake and genuine data from the training and test sets are concatenated to create the final training and test sets. Labels are also assigned (0 for fake, 1 for genuine).

Splitting the Dataset
The dataset is split into training and testing sets using the train_test_split function from scikit-learn.

Defining the CNN Model
A simple CNN model is defined using the Keras Sequential API. It consists of convolutional layers, max-pooling layers, and dense layers.

Compiling the Model
The model is compiled with the Adam optimizer and binary cross-entropy loss, as it is a binary classification problem. The accuracy metric is used for evaluation.

Training the Model
The model is trained on the training set with 10 epochs and a batch size of 32. Validation data is used to monitor the model's performance during training.

Evaluating the Model
The trained model is evaluated on the test set, and accuracy along with the confusion matrix is printed.
![WhatsApp Image 2024-06-21 at 12 01 50_3b9ddf18](https://github.com/charangangula/fake-logo-detection/assets/172465090/53217120-f616-4455-9496-28b3f9ea8799)
![WhatsApp Image 2024-06-21 at 12 03 28_876fdfde](https://github.com/charangangula/fake-logo-detection/assets/172465090/f20c80c8-9cf7-493c-a6e1-2e758d7a615a)

CNN-CIFAR10 Image Classification

A Convolutional Neural Network (CNN) trained on the CIFAR-10 dataset to classify images into 10 object categories.
This project includes model building, training, evaluation, and visualizations such as accuracy/loss curves and a confusion matrix.

Dataset: CIFAR-10

CIFAR-10 contains 60,000 color images (32×32) across 10 classes:

| airplane | automobile | bird | cat | deer |
| dog | frog | horse | ship | truck |

50,000 images → Training

10,000 images → Testing

Model Architecture

The CNN consists of data augmentation, three convolutional blocks, and dense layers:

🔹 Data Augmentation

Random Flip

Random Rotation

Random Zoom

3 Convolution Blocks

Conv2D → BatchNorm → Conv2D → BatchNorm → MaxPooling → Dropout

Fully Connected Layers

Dense(128, relu) + Dropout(0.5)

Dense(10, softmax)

The model is trained using:

Optimizer: Adam

Loss: Sparse Categorical Crossentropy

Batch Size: 64

Epochs: 20–30
Model Performance

Typical performance after training:

Training Accuracy: ~85%

Test Accuracy: ~75–80%

Included Visualizations

✔ Training vs. Validation Accuracy
✔ Training vs. Validation Loss
✔ Confusion Matrix


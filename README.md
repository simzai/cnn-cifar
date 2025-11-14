# cnn-cifar
This project builds and trains a Convolutional Neural Network (CNN) to classify images from the CIFAR-10 dataset into 10 categories. The model uses data augmentation, Batch Normalization, Dropout, and a multi-layer CNN architecture to achieve high accuracy.

CIFAR-10 contains 60,000 color images (32×32 px) across 10 classes:

airplane

automobile

bird

cat

deer

dog

frog

horse

ship

truck

50,000 images → training
10,000 images → testing

The project uses a deep CNN with:

Data Augmentation

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

Training Accuracy: ~85% (depending on number of epochs)

Test Accuracy: ~75–80%

Includes:

Accuracy graph

Loss graph

Confusion matrix


MNIST Image Classification with CNN
Project Goal

The main objective of this project is to perform image classification of handwritten digits using a Convolutional Neural Network (CNN).
Dataset

The MNIST dataset was used for training and evaluating the model.
Model Architecture

The CNN model architecture consists of the following layers:

    Convolutional layer with 32 filters, 3x3 kernel, and ReLU activation.
    Dropout layer with a rate of 0.2.
    MaxPooling layer with a 2x2 pool size.
    Convolutional layer with 64 filters, 3x3 kernel, and ReLU activation.
    MaxPooling layer with a 2x2 pool size.
    Convolutional layer with 64 filters, 3x3 kernel, and ReLU activation.
    MaxPooling layer with a 2x2 pool size.
    Flatten layer.
    Dense layer with 64 units and ReLU activation.
    Dense output layer with 10 units and Softmax activation.

Training Details

    Optimizer: Adam
    Loss Function: Categorical Crossentropy
    Metrics: Accuracy
    Epochs: 10
    Batch Size: 128
    Validation Strategy: 20% of the training data was used for validation.
    Callbacks: TensorBoard was used for logging.

Results

The model achieved a test accuracy of approximately 0.9857.
Observations and Future Work

A slight increase and fluctuation in validation loss were observed between epochs 6 and 8. This raises questions about potential overfitting and whether this fluctuation is normal.

Potential areas for hyperparameter tuning to improve performance include:

    Number of Epochs
    Batch Size
    Number and size of Layers (e.g., increasing the third convolutional layer's filters)
    Strides
    Optimizer (e.g., trying RMSprop)

Further concepts to understand and potentially implement include:

    Padding
    Batch Normalization
    Image Rotation
    Dropout (further tuning the rate or placement)

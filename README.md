HybridConvNet – Skin Disease Classification
This project focuses on identifying skin diseases using deep learning. Our goal was to correctly classify images of Monkeypox, Measles, and Chickenpox using computer vision techniques.

What We Tried
We started by testing some popular deep learning models on their own:

Inception V3

DenseNet121

MobileNetV3-Large

EfficientNet-B0

However, the results from these individual models were not satisfactory. They did not perform well enough on our dataset and failed to give consistent accuracy.

What We Built
To solve this issue, we created our own model by combining three different models into one. This new model is called HybridConvNet.

HybridConvNet works by:

Taking features from DenseNet121, MobileNetV3-Large, and EfficientNet-B0

Merging the best parts of each model

Using those combined features to make final predictions

This approach helped the model learn better from the images and improved the overall performance.

Results
Our custom HybridConvNet achieved an accuracy of above 98 percent on the test set. It was able to classify the skin diseases more accurately than the single models we tried earlier.

We also included tools to:

Show how accurate the model is

Display a confusion matrix to visualize predictions

Generate ROC curves to understand the performance for each class

How the Model Was Trained
The dataset was split into training, validation, and test sets.

The model was trained for 30 rounds (epochs).

Images were resized and slightly changed (flipped, rotated, adjusted) to make the model more robust.

We tracked both training and validation accuracy over time.

After training, we tested the model and saved it for future use.

How to Use
Place your dataset in the correct folders for training and testing.

Run the training script to train the model.

Use the saved model to test new images or continue improvements.

Final Notes
This project shows that combining models can be more effective than using a single one. Our HybridConvNet learns better by using the strengths of different models together. It is especially useful for detecting similar-looking diseases like Monkeypox and Chickenpox.

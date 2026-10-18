Understanding Uncertainty and Accuracy in an Image Classifier

This notebook trains an image classifier that classifies high-rise buildings from low-rise houses. Following which an uncertainty analysis is taken to evaluate confidence and accuracy scores to understand:

1\. Model behaviour and performance against different image categories

2\. How to correctly interpret accuracy and confidence scores

3\. The uncertainty range of model accuracy



Why this matters: Understanding accuracy and confidence in detail highlights the model's strengths and weaknesses. This helps users decide when to trust a prediction, and when to check it, before using the model in future applications.



How it works

1. Download training images from the Wikimedia Commons API, one folder per class.
2. Train the model with fastai, fine-tuning a pretrained ResNet34.
3. Download new test images, label each one by hand, and record the model's predictions and probabilities.
4. Analyse uncertainty: confusion matrix, confidence histograms, bootstrap intervals for accuracy and recall, and calibration checks.



How to run

1. Open the notebook on Kaggle.
2. In the notebook settings, turn Internet on.
3. Run steps 1 to 3 in order. Step 3.2 asks you to click a label for each test image.
4. Step 4 can also run on its own using the saved results file, r2\_df\_uncertainty.csv.

All required packages come pre-installed on Kaggle.



Data and licences

Images come from Wikimedia Commons. Each image has its own licence, and most require attribution. Images are not stored in this repository; the notebook downloads them.


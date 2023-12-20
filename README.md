face mask detection using opencv

The project employs OpenCV for face mask detection. The code snippet initializes using NumPy and OpenCV libraries. It loads two NumPy arrays, one containing images of faces with masks and another with faces without masks. These arrays are reshaped for compatibility, combined into a single feature dataset (X), and labeled (0 for masks, 1 for no masks).

A Support Vector Classifier (SVC) model is utilized for training, where the images are split into training and testing sets. Principal Component Analysis (PCA) is applied for dimensionality reduction before training the SVC model. The accuracy score is calculated to evaluate the model's performance on the test set.

The code also implements live face detection from a webcam feed using Haar Cascade classifiers. Detected faces are outlined, cropped, resized, and used to predict mask or no mask using the trained SVC model. The predicted labels are displayed in real-time on the video feed.

The project showcases a workflow starting from data preparation, model training, and evaluation, culminating in real-time mask detection from a live video feed using OpenCV and machine learning techniques.

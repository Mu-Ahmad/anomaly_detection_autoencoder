# anomaly_detection_autoencoder

Anomaly detection refers to the task of finding/identifying rare events/data points. Some applications include - bank fraud detection, tumor detection in medical imaging, and errors in written text. A lot of supervised and unsupervised approaches to anomaly detection has been proposed. Some of the approaches include - One-class SVMs, Bayesian Networks, Cluster analysis, and (of course) Neural Networks.

We will use an Autoencoder Neural Network to detect/predict anomalies in ECG


Autoencoders Neural Networks try to learn data representation of its input. So the input of the Autoencoder is the same as the output? Not quite. Usually, we want to learn an efficient encoding that uses fewer parameters/memory. The encoding should allow for output similar to the original input. In a sense, we’re forcing the model to learn the most important features of the data using as few parameters as possible.

Here are the basic steps to Anomaly Detection using an Autoencoder:

Train an Autoencoder on normal data (no anomalies)
Take a new data point and try to reconstruct it using the Autoencoder
If the error (reconstruction error) for the new data point is above some threshold, we label the example as an anomaly


![1*525GY1x9cGY2E7fXW5qk_w](https://user-images.githubusercontent.com/58839486/188960692-1a8a1408-0eb2-4086-8c31-1a2d51355230.png)

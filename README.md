# MNIST Neural Network from Scratch

In this project, I built a two-layer feedforward neural network entirely from scratch to recognize MNIST digits (0-9). I built this without using any high-level machine learning frameworks like TensorFlow or PyTorch—relying only on Python, NumPy, and the underlying mathematics.

## What I Did

* **Data Processing:** Loaded the MNIST dataset (via CSV in Google Colab), split the data into training and validation sets, and normalized the pixel values to prevent math overflow errors.
* **Forward Propagation:** Implemented the dot products and activation functions to make predictions.
  * **Hidden Layer:** 10 nodes using a **ReLU** activation function.
  * **Output Layer:** 10 nodes using a **softmax** activation function to output probabilities for digits 0-9.
* **Backward Propagation:** Brute-forced the calculus and derivatives to calculate the error gradients (`dW1, dB1, dW2, dB2`) using categorical cross-entropy and one-hot encoding.
* **Gradient Descent:** Built the training loop to update the weights and biases over multiple iterations based on a set learning rate.
* **Visualization & Testing:** 
  * Wrote a function to test the model on validation data, reshape the 784-pixel vectors back into 28x28 images, and plot them using Matplotlib alongside the model's prediction.

## Technologies Used
* **NumPy:** For all matrix math, dot products, and gradient calculations.
* **Pandas:** For loading and manipulating the CSV dataset.
* **Matplotlib:** For rendering the 28x28 pixel arrays as viewable images.
* **Google Colab:** Used as the environment, pulling the dataset directly from Google Drive.

*A breakdown of all the mathematics used can be found in the MATH-NOTES file.*

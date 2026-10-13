# Deep Learning and Computer Vision

Notebooks from my *Introduction to AI* and *Computer Vision* courses at Egypt University of Informatics, covering neural network classification and motion estimation.

| Notebook | Topic | Result |
|---|---|---|
| [`cnn_mnist_classification.ipynb`](cnn_mnist_classification.ipynb) | Handwritten digit recognition on MNIST. Starts with a dense baseline, then builds a CNN (Conv2D → MaxPooling → Dense) in Keras, with training curves, a confusion matrix and predictions on random test images | **97.5%** test accuracy (CNN) |
| [`iris_neural_network.ipynb`](iris_neural_network.ipynb) | Multi-class classification of the Iris dataset with a feed-forward neural network (StandardScaler preprocessing, 2 hidden ReLU layers, softmax output). The trained model is saved as `iris_model.h5` | **100%** test accuracy |
| [`lucas_kanade_optical_flow.ipynb`](lucas_kanade_optical_flow.ipynb) | Lucas–Kanade optical flow implemented by hand: Shi–Tomasi corner detection, Sobel spatial and temporal gradients, and a least-squares solution of the flow equations per window. Compared against OpenCV's pyramidal `calcOpticalFlowPyrLK` | Motion vectors visualized on consecutive video frames |

## Run

Run the notebooks in Google Colab or Jupyter. They need:

```bash
pip install tensorflow scikit-learn numpy pandas matplotlib opencv-python
```

The optical flow notebook expects two consecutive frames, `basketball1.png` and `basketball2.png`, in the working directory. Any two consecutive grayscale video frames will work.

## Tech

Python · TensorFlow/Keras · scikit-learn · OpenCV · NumPy · Matplotlib

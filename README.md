# Brain-tumor-detection
This project focuses on detecting brain tumors from MRI scans using deep learning, specifically through transfer learning with the VGG16 architecture. The model leverages a pretrained VGG16 network from ImageNet, which is fine-tuned to classify brain MRI images into two categories: Tumor and No Tumor. This approach improves performance and reduces training time by using previously learned visual features.

The dataset used for this project includes brain MRI images labeled according to the presence or absence of a tumor. These images are preprocessed to match VGG16’s input requirements — resized to 224x224 pixels, normalized, and augmented to enhance generalization. The model replaces VGG16's top layers with a custom classification head comprising dense layers, dropout, and a sigmoid output neuron for binary classification.

The project is implemented entirely in Python using TensorFlow/Keras along with supporting libraries like NumPy, Matplotlib, and scikit-learn. Training and evaluation are conducted in a single script or notebook, and the model achieves high accuracy on the test set, often exceeding 95% depending on the dataset used. The notebook also includes visualizations for training loss, accuracy, and sample predictions.

This project is useful for demonstrating how to apply transfer learning in a medical imaging context using minimal code and resources. It can be run on platforms like Google Colab for quick GPU-accelerated training. The repository includes the training code and guidance for dataset preparation, making it a great starting point for further development in medical image classification.



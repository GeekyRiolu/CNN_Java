# Java Neural Network for MNIST Dataset

This project is a Java-based implementation of a Convolutional Neural Network (CNN) designed to classify handwritten digits from the MNIST dataset. The project trains the neural network using the MNIST training dataset and evaluates its accuracy using the test dataset.

## Features
- Supports convolutional and max-pooling layers.
- Fully connected layers for classification.
- Trains on the MNIST dataset for digit recognition.
- Evaluates and prints the success rate before and after training.

## Prerequisites
To run this project, ensure you have the following:
- Java Development Kit (JDK) 8 or above installed.
- The MNIST dataset in CSV format:
  - `mnist_train.csv` for training.
  - `mnist_test.csv` for testing.
- Dependencies:
  - `data.DataReader`: Reads the MNIST CSV data.
  - `network.NetworkBuilder`: Builds the neural network.
  - `network.NeuralNetwork`: Represents the neural network.

## How It Works
1. **Data Loading**: The program reads the MNIST training and testing datasets from the `data` directory.
2. **Network Construction**: The network consists of:
   - A convolutional layer with 8 filters.
   - A max-pooling layer.
   - A fully connected layer with 10 outputs (for digits 0–9).
3. **Training**: The network is trained for a specified number of epochs on the training dataset.
4. **Testing**: The program evaluates the success rate on the test dataset before and after training.

## How to Run
1. **Set Up the Environment**:
   - Clone the repository or copy the project files to your local machine.
   - Ensure the `mnist_train.csv` and `mnist_test.csv` files are placed in the `data` directory.

2. **Compile and Run**:
   - Navigate to the `src` directory and compile the code:
     ```bash
     javac Main.java
     ```
   - Run the program:
     ```bash
     java Main
     ```

3. **Output**:
   - The program prints the success rate before and after each epoch.

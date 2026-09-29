# AIML-Recruitment-2026-<YourName>

## 1. Candidate Details
- **Name:** <Your Full Name>
- **Year / Branch:** Second Year, <Your Branch>
- **University:** SRM Institute of Science and Technology
- **Registration No.:** <Your Reg No.>
- **Email / Contact:** <Your Email>

## 2. Tasks Completed
- [ ] Task 1: Air Quality Forecasting
- [x] Task 2: Neural Network (MNIST)

## 3. Problem Statement
Classify 28x28 grayscale images of handwritten digits (0-9) using a simple neural network, and analyse how changing the model affects performance.

## 4. Approach
1. **Understood the data:** 60,000 training and 10,000 test images, 10 classes, checked class balance.
2. **Preprocessed:** normalised pixels from 0-255 to 0-1 and flattened 28x28 images to 784-value vectors.
3. **Built the model:** Input (784) -> Dense(128, ReLU) -> Dense(10, Softmax) using Keras.
4. **Trained:** Adam optimizer, sparse categorical cross-entropy loss, 10 epochs, batch size 32.
5. **Evaluated:** accuracy, confusion matrix, precision/recall/F1.
6. **Experimented:** reduced hidden neurons from 128 to 32 and compared the results.

## 5. Technologies Used
Python, TensorFlow/Keras, NumPy, Pandas, Matplotlib, Seaborn, scikit-learn, Google Colab, Git/GitHub.

## 6. Results
| Model | Parameters | Train Acc | Val/Test Acc | Train Loss | Val/Test Loss |
|---|---|---|---|---|---|
| Baseline (128 neurons) | <fill> | <fill> | <fill> | <fill> | <fill> |
| Experiment (32 neurons) | <fill> | <fill> | <fill> | <fill> | <fill> |

- Most confused digits: <fill from your confusion matrix, e.g. 4 vs 9>
- Experiment outcome: <one sentence on what changed and why>

## 7. Key Learnings
1. Neural networks need **non-linear activation functions** (like ReLU) to learn complex patterns; softmax turns outputs into class probabilities.
2. **Preprocessing matters:** normalising inputs helps the model train faster and more stably.
3. **Accuracy alone is not enough:** a confusion matrix shows which classes get confused with each other.
4. <Add your own learning, e.g. about model capacity / overfitting>

## 8. Challenges
- **Challenge:** <e.g. Understanding what softmax and loss actually do>
- **How I solved it:** <e.g. Plotted a small softmax example by hand and read the Keras docs>

## Files
- `MNIST_Neural_Network.ipynb`: full notebook with outputs
- `README.md`: this file

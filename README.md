# AIML-Recruitment-2026-AYUSH AGARWAL    

## 1. Candidate Details
- **Name:** Ayush Agarwal
- **Year / Branch:** Second Year, B.Tech CSE Core
- **University:** SRM Institute of Science and Technology
- **Registration No.:** RA2511003010012  
- **Email / Contact:** aa3098@srmist.edu.in

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
| Baseline (128 neurons) | 101,770 | 0.9962 | 0.9753 | 0.0133 | 0.0968 |
| Experiment (32 neurons) | 25,450 | 0.9808 | 0.9671 | 0.0694 | 0.1207 |

- Most confused digits: true 0 predicted as 6 (13 cases), true 5 predicted as 3 (13 cases), true 2 predicted as 7 (11 cases), true 4 predicted as 9 (11 cases)
- Experiment outcome: reducing the hidden layer from 128 to 32 neurons cut the parameters by about 75% (101,770 to 25,450) and lowered validation accuracy from 97.5% to 96.7%, showing that fewer neurons give the model less capacity to learn digit patterns.
## 7. Key Learnings
1. Neural networks need **non-linear activation functions** (like ReLU) to learn complex patterns; softmax turns outputs into class probabilities.
2. **Preprocessing matters:** normalising inputs helps the model train faster and more stably.
3. **Accuracy alone is not enough:** a confusion matrix shows which classes get confused with each other.
4. 4. Model capacity matters, but with diminishing returns: cutting the hidden layer size by 75% only reduced accuracy by about 1 percentage point, and the smaller model also showed a slightly smaller train-validation gap, meaning less overfitting.

## 8. Challenges
- **Challenge:** Understanding why ReLU and softmax are used in different layers, and what the confusion matrix numbers actually meant beyond a single accuracy score.
- **How I solved it:** Plotted the ReLU function and a small softmax example by hand, and read through the Keras documentation and the classification report to interpret precision, recall and F1 per digit.

## Files
- `MNIST_Neural_Network.ipynb`: full notebook with outputs
- `README.md`: this file

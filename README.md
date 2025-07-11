# Human-Activity-Recognition-System
This project uses simulated sensor data to classify six human activities with a CNN model. Activities include Squats, Jumping Jacks, Push-ups, Walking, Sitting, and Sleeping. It achieves high accuracy and includes voice feedback using gTTS, demonstrating the potential of deep learning in Human Activity Recognition.



## **Project Overview**

### **Title:**

**Human Activity Recognition Using Machine Learning Techniques**

### **Objective:**

To build a simulation-based Human Activity Recognition system that classifies six different physical activities using synthetic sensor signals and a deep learning model (CNN), and delivers real-time voice feedback using Google Text-to-Speech (gTTS).

---

### **Activities Recognized:**

* Squats
* Jumping Jacks
* Push-ups
* Walking
* Sitting
* Sleeping

---

### **Key Components:**

#### 1. **Simulated Sensor Data**

Rather than using physical sensors or pre-recorded datasets, the project generates artificial time-series data that mimic accelerometer signals for each activity using sine wave functions and Gaussian noise.

#### 2. **Data Preprocessing**

* Signal normalization (StandardScaler)
* Label encoding and one-hot transformation
* Data reshaping for CNN input
* 70:30 train-test split

#### 3. **Model Architecture**

A 1D Convolutional Neural Network (CNN) is used, featuring:

* Two convolutional layers
* Max pooling
* Dropout for regularization
* Dense layers with ReLU and softmax activation

The model is trained using categorical cross-entropy loss and the Adam optimizer.

#### 4. **Evaluation Metrics**

* Accuracy
* Confusion Matrix
* Precision, Recall, F1-Score (via Classification Report)

#### 5. **Voice Feedback System**

A speech output system using `gTTS` allows the model to **announce the predicted activity**, enhancing interactivity—especially within Google Colab environments.

---

### **Results Summary:**

* High classification accuracy across all six activities.
* Minor confusions occurred in low-motion classes (e.g., Sitting vs. Sleeping).
* The CNN effectively learned to differentiate activity patterns from synthetic signals.

---

### **Applications:**

* Fitness monitoring
* Remote elderly care systems
* Smart home interaction
* Educational demonstrations of HAR systems

---

### **Future Enhancements:**

* Replace simulated data with real-world sensor inputs (e.g., UCI HAR or WISDM datasets)
* Explore temporal models like LSTM or CNN-LSTM hybrids
* Deploy the system on mobile or wearable platforms for real-time recognition


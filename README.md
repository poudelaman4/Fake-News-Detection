### Fake News Detection Project

This project aims to detect fake news using machine learning and deep learning techniques. The goal is to classify news articles as either **fake** or **true** based on their text content.

---

### **Models and Results**

The analysis in this project utilizes two distinct models to classify news articles. The results below showcase the performance of each model on the test data.

#### **Logistic Regression**

A **Logistic Regression** model was trained on the preprocessed text data. This model serves as a strong baseline for text classification.

* **Accuracy:** **98.6%**
* **Classification Report:**
    * **Precision:**
        * Fake: 0.99
        * True: 0.98
    * **Recall:**
        * Fake: 0.98
        * True: 0.99
    * **F1-Score:**
        * Fake: 0.98
        * True: 0.99

#### **LSTM (Long Short-Term Memory) Neural Network**

A deep learning model using a **Bidirectional LSTM** was also implemented. This model is capable of capturing sequential dependencies in the text, which is highly effective for natural language processing tasks.

* **Accuracy:** **99.5%**
* **Classification Report:**
    * **Precision:**
        * Fake: 1.00
        * True: 0.99
    * **Recall:**
        * Fake: 0.99
        * True: 1.00
    * **F1-Score:**
        * Fake: 0.99
        * True: 1.00

---

### **Conclusion**

The **LSTM model** demonstrated superior performance, achieving a final accuracy of **99.5%**. This is a significant improvement over the Logistic Regression baseline and highlights the power of deep learning for text classification. The results confirm that the model is highly effective at distinguishing between fake and real news articles.

---

### **Project Process**

1.  **Data Preprocessing**: The project began with data loading, combining separate fake and real news datasets, and adding a `label` column for classification. A `full_text` column was then created by merging the title and body of each article.
2.  **Model Training**: The preprocessed data was used to train both the Logistic Regression and LSTM models, with the latter built using `TensorFlow` and `Keras`.

---

### **Getting Started**

To run this project, you will need the following libraries:
* `pandas`
* `numpy`
* `scikit-learn`
* `tensorflow`
* `keras`

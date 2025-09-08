# 📧 Spam Email Classification Lab

We are Group 9 in Class 23TNT1 at Ho Chi Minh City University of Science.
Rather than just using ready-made libraries, we challenged ourselves to go back to the foundations of Machine Learning — building a Naive Bayes Spam Classifier from scratch and putting it to the test on real-world email data.

This project has been both fun and eye-opening, giving us a taste of how classic ML algorithms still shine in today’s AI world.

Thanks for stopping by our repo 🚀.
We’d love to hear your feedback, ideas, or even spam jokes 💌.

Best wishes and happy coding from Group 9! 🎉

---

## 📊 Dataset
- **Source**: Enron-Spam dataset (provided via Moodle/Google Drive, therefore not included in this repository).  
- **Content**:
  - **Subject**: Email subject line.  
  - **Message**: Body of the email (can be empty in some cases).  
  - **Label**: `"spam"` or `"ham"`.  

- **Files**:
  - `train.csv`: Training set.  
  - `val.csv`: Validation set.  

---

## 🛠 Workflow  

1. **Data Loading**  
   - Load train and validation datasets.  
   - Display dataset information and preview first 5 rows.  

2. **Preprocessing**  
   - Handle duplicates and missing values.  
   - Shuffle and merge datasets if needed.  
   - Tokenize and clean text.  
   - Encode labels into numerical values.  

3. **Model Training**  
   - Implement **Naive Bayes Classifier** (Multinomial).  
   - Derive model using **Maximum Likelihood Estimation (MLE)** and **Maximum A Posteriori (MAP)**.  
   - Train on `train.csv`.  

4. **Evaluation**  
   - Evaluate on both training and validation sets.  
   - Report metrics: **Accuracy, Precision, Recall, F1-score**.  

5. **Real-world Testing**  
   - **Function 1**: Allow user to input custom email (subject + body) → predict spam/ham.  
   - **Function 2**: Allow user to upload custom CSV file (same format as `val.csv`) → evaluate model on it.  

---

## 📈 Results  

**Training set**:  
- Accuracy: **98.93%**  
- Precision: **98.86%**  
- Recall: **99.03%**  
- F1-Score: **98.95%**  

**Validation set**:  
- Accuracy: **98.51%**  
- Precision: **98.53%**  
- Recall: **98.53%**  
- F1-Score: **98.53%**  

👉 The model performs excellently with >98% on all metrics for both training and validation, showing strong generalization ability.  

---

## 🚀 How to Run
```bash
# Install dependencies
pip install -r requirements.txt

# Launch notebook
jupyter notebook notebook/Source.ipynb
# spam-classification-lab
Naive Bayes Spam Classifier built from scratch using the Enron-Spam dataset.  Includes data preprocessing, model training &amp; evaluation, and real-world testing with custom emails.

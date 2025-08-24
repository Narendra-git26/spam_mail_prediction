# spam_mail_prediction
spam mail  prediction 
A lightweight, end-to-end machine-learning project that classifies emails as Spam or Ham (Not Spam). Trained on labeled email text, the model achieves 96% accuracy on the training set and 95% accuracy on the held-out test set, balancing precision and recall to minimize both false alarms and missed spam.

✨ Highlights

Problem: Binary text classification — detect spam emails from their content/metadata.

Approach: Classic NLP pipeline with text cleaning → vectorization → supervised classifier.

Performance:

Train Accuracy: 96%

Test Accuracy: 95%

Robust generalization with low overfitting.

Reproducible: Deterministic preprocessing and train/test split.

Deployable: Exposes a simple prediction interface you can plug into apps, CLIs, or APIs.

🧠 Model Overview

Preprocessing

Lowercasing, punctuation & digit cleanup

Stop-word removal

Optional lemmatization

Feature Extraction

TF-IDF (unigrams/bigrams), max-features tuned for performance vs. size

Classifier

A strong linear baseline (e.g., Logistic Regression / Linear SVM) or Multinomial Naive Bayes

Calibrated decision thresholds (optional) to balance precision/recall

The exact model and hyperparameters are captured in the accompanying notebook: spam_mail_prediction.ipynb.

## Installation

Clone the repository and install the required packages:

```bash
git clone https://github.com/<your-username>/spam-mail-prediction.git
cd spam-mail-prediction
pip install -r requirements.txt


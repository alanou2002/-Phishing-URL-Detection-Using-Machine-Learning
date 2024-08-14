# Phishing-URL-Detection-Using-Machine-Learning
This project develops machine learning models to detect phishing URLs in emails, using features like URL structure and domain characteristics. We implemented logistic regression for interpretability and Random Forest for high accuracy, achieving up to 98.77% accuracy.

## Motivation
The rise of online communication platforms like email has significantly improved global connectivity but also opened doors for malicious activities like phishing. Phishing emails trick users into divulging sensitive information or installing malware by mimicking legitimate services. Current solutions, such as educating users and spam filters, are insufficient, especially for vulnerable populations. This project leverages machine learning to classify embedded URLs in emails as either phishing or legitimate.

## Data
The dataset used is a collection of features from URLs, specifically designed for phishing detection. Key features include the number of special characters, domain length, server-client relationships, time domain activation, TTL hostname, TLS SSL certificate status, and whether the URL was indexed by Google.

Preprocessing steps included:
- Removal of missing values.
- Ensuring balanced classes.
- Dropping features with no variance and categorical variables with excessive unique values.

## Models
### Logistic Regression
- **Baseline Model:** 
  - Accuracy: 91.17%
  - ROC-AUC: 0.9705
- **L1 Regularized Model:**
  - Accuracy: 91.97%
  - ROC-AUC: 0.974

### Random Forest
- **Baseline Model:** 
  - Accuracy: 98.77%
  - ROC-AUC: 0.998
- **Feature-Selected Model:**
  - Accuracy: 98.66%
  - ROC-AUC: 0.998

Random Forest models outperformed logistic regression in accuracy and handling complex data, though logistic regression provided more interpretability. Future improvements could include hyperparameter tuning, additional feature selection techniques, and real-time testing.

## Impact
Our model demonstrates high accuracy in detecting phishing URLs, contributing to enhanced cybersecurity. It can be particularly useful in high-risk industries like banking and e-commerce, as well as for less tech-savvy populations. Future versions could incorporate text analysis, cross-industry collaborations, and expanded feature sets for even greater accuracy and adaptability to evolving threats.

# Network-Intrusion-Detection-System
*Cyber Security Project Using Machine Learning*
Network Intrusion Detection System
This project analyzes network traffic data to detect and classify cyber attacks using Machine Learning. It utilizes the NSL-KDD dataset to categorize network activity into normal traffic or specific attack types.

📌 Project Overview
Goal: Classify network connections as Normal, DoS, Probe, R2L, or U2R.

Model Used: Random Forest Classifier.

Performance: Achieved ~99% accuracy on the test split.

⚙️ Key Steps
Data Preprocessing:

Mapped specific attack labels (e.g., neptune, satan) to broader categories (DoS, Probe, etc.).

Encoded categorical features (protocol_type, service, flag) using OneHotEncoder.

Model Training:

Trained a Random Forest Classifier (n_estimators=300).

Utilized class weighting to handle imbalanced data.

Evaluation:

Generated Classification Reports and Confusion Matrices.

Visualized the Top 20 Important Features affecting the classification.

🛠️ Requirements
To run this notebook, you need Python and the following libraries:

pandas

numpy

scikit-learn

matplotlib

joblib

📊 Results
The model successfully identifies network intrusions with high precision, identifying features like src_bytes, dst_bytes, and traffic count as the most significant indicators of an attack.

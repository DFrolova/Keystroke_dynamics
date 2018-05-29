# Keystroke_dynamics
Different algorithms for user authentication based on keystroke dynamics of a user of mobile phone

Here different algorithms of anomaly detection are tested in order to get best performance in making decisions whether the user is normal or he is illegal. EER (equal error rate) is percent or errors when FAR = FRR (type I and II errors).

There are statistical ones:
- Creating a template of mean +- std of each feature in feature-vector based on training set. EER = 8.0%.
- Creating a template of mean value of each feature and counting distance from template to vector being tested. Decision is taken based on the threshold distance? than is counted as a 10%-percentile on training set. EER = 11.2% for manhattan metric and 16.1% for euclidean metric.
- Isolation Forest. EER = 12.1%.
- One-class SVM. EER = 14.9%.
- Local Outlier Factor - density-based anomaly detection algorithm based on analysys of k nearest neighbours. For manhattan metric EER = 12.7%, for euclidean metric EER = 16.5%.

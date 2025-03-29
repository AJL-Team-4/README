# README
Contributors:
- Jun Ze He
   - https://github.com/JunJul
- Andrew Lam
  - https://github.com/anlam35705
- Camille Dove
  - https://github.com/CamilleDove
- Melissa April
  - https://github.com/melissaaapril

Project Overview:

- This Kaggle competition is part of the Break Through Tech AI Program in collaboration with the Algorithmic Justice League. The challenge focuses on improving AI fairness in dermatology by developing an inclusive machine-learning model that can classify 21 different skin conditions across diverse skin tones.

Objective of the Challenge:

- The primary goal is to train an AI model that accurately classifies skin conditions while ensuring equitable performance across different skin tones. The competition evaluates submissions based on a weighted F1 score to account for class imbalances.

Real-World Significance & Impact:

- Many existing dermatology AI tools underperform for people with darker skin tones due to biased training data, leading to misdiagnoses and health disparities. By building a more inclusive model, this project aims to contribute to more equitable healthcare outcomes, ensuring timely and accurate skin condition diagnoses for historically underserved communities. Additionally, participants will document their process using fairness and explainability tools to highlight AI biases and promote transparency in medical AI applications.

Data Exploration:

- The dataset is a subset of the FitzPatrick17k dataset, a labeled collection of about 17,000 images depicting a variety of serious (e.g., melanoma) and cosmetic (e.g., acne) dermatological conditions with a range of skin tones scored on the FitzPatrick skin tone scale (FST). About 4500 images are in this set, representing 21 skin conditions out of the 100+ in the full FitzPatrick set.

Data Cleaning:
- Identified missing values, particularly in the 'qc' column.

- Removed rows marked as "3 Wrongly labelled" to eliminate incorrectly labeled data.

- Dropped the now-unnecessary 'qc' column.

- Checked for duplicate entries to ensure data integrity.

Label Encoding:
- Sorted the unique labels to enforce a consistent order.

- Used scikit-learn’s LabelEncoder to transform the labels into numeric values.

- Converted the numeric labels to strings to ensure compatibility with Keras's ImageDataGenerator when using class_mode='categorical'.

Data Visualization:

- Class distribution plots were created to visualize the frequency of each skin condition.

- Examined skin tone distributions using histograms for self-reported and centaur-assigned Fitzpatrick scales.

![image](https://github.com/user-attachments/assets/1c3f9bb4-85a3-4348-b543-f4c7fd8ddb69)
![image](https://github.com/user-attachments/assets/fdac011e-3846-48cb-9fd0-cc81fc68ff9b)

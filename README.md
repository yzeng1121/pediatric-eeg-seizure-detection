# Detection of Epilepsy and Seizure Using EEG Scans
Detection of Epilepsy and Seizure Using EEG Scans

## Research Question
Can convolutional neural networks (CNNs) achieve diagnostic accuracy comparable to traditional clinical methods in detecting epileptic seizures from EEG data?

## Summary
Epilepsy affects millions worldwide, and timely diagnosis is crucial for effective treatment. Traditional diagnostic methods often require extensive EEG review by specialists, which is both time-consuming and expert-intensive, and not to mention expensive. According to Temple (2024), a 2020 study found that $8.6 billion was spent on epilepsy-related costs, with 40% of this amount not covered by public insurance. Even before treatment is given out, it takes anywhere from 3 days to a week for paroxysmal seizures to be diagnosed (Friedman, Hirsch, 2009). Our project aims to evaluate whether convolutional neural networks (CNNs) can accurately classify epileptic seizure activity from pre-existing, labeled EEG data, potentially streamlining diagnostic processes and increasing access to early detection tools.

Using several open-source EEG datasets, we will train and test a CNN model on labeled brain activity associated with seizures and non-seizures. We will compare its performance (accuracy, sensitivity, specificity, F1 score) against benchmarks established in prior medical literature and explore how model predictions might supplement or approximate the diagnostic process of a human clinician.

Our goal is to determine whether CNN-based systems can provide a fast and cost-effective screening tool to assist in early seizure detection, particularly in settings where neurologists or EEG specialists are limited, such as rural or low-income communities.

## Datasets
We plan to use the following datasets from Kaggle to train our CNN model:
- Seizure Epilepsy CHB MIT EEG dataset pediatric
- Siena Scalp EEG Database

These datasets include EEG scans labeled for seizure and non-seizure events, providing diverse demographic and physiological samples for model generalization.

## Machine Learning Algorithm to be Used
We will be using convolutional neural networks (CNNs) and experimenting with different architectures and hyperparameters to optimize classification performance. CNNs were chosen because they do not require any domain knowledge or manual feature extraction. Instead of handcrafting features from EEG signals, the model can automatically learn patterns directly from the raw or minimally processed data. Comparisons may also be made to baseline models (e.g., Decision Trees or Random Forests) for context.

## Sources of Bias
- Demographic variability: different datasets originate from varying populations (pediatric vs. adult, Turkish vs. international subjects), which could introduce population bias
- Data imbalance: some datasets contains more non-seizure EEG samples than seizure ones, leading to skewed model performance
- EEG equipment and preprocessing differences: variations in electrode placement or signal filtering can affect model generalization
- Labeling inconsistencies: mislabeling or differing clinical criteria for seizures may distort training accuracy

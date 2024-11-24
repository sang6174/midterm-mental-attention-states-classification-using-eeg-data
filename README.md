MIDTERM - Mental Attention States Classification Using EEG DATA

I. Obbjective
Classify mental attention states (focused, unfocused, drowsy) based on EEG signals using machine learning techniques.

II. Dataset Detail
1. Dataset source
- Dataset URL: https://www.kaggle.com/datasets/inancigdem/eeg-data-for-mental-attention-state-detection/data
- Data was acquired from EMOTIV EEG devices during 34 experiments.
- EEG data is in channels 4 to 17 of the provided Matlab files.
- Sampling frequency: 128 Hz.

2. Context
This is a collection of 34 experiments for monitoring of attention state in human individuals using passive EEG BCI.
Each Matlab file contains the object of the data acquired from EMOTIV device during one experiment. The raw data is contained in o.data, which is array of size {number-of-samples}x25, thus o.data(:,i) comprises one data channel. The sampling frequency is 128 Hz. The list of data channels and their numerical ids is given below per EMOTIV documentation;

1-'ED_COUNTER' - A counter or index of a data sample. helps track the order of records in a time series. \
2-'ED_INTERPOLATED' - Flag indicating if data has been interpolated to fill gaps or missing data. \
3-'ED_RAW_CQ' - Raw signal quality index, reflecting the level of noise or clean signal. \
4-'ED_AF3' \
5-'ED_F7' \
6-'ED_F3' \
7-'ED_FC5' \
8-'ED_T7' \
9-'ED_P7' \
10-'ED_O1' \
11-'ED_O2' \
12-'ED_P8' \
13-'ED_T8' \
14-'ED_FC6' \
15-'ED_F4' \
16-'ED_F8' \
17-'ED_AF4' \
18-'ED_GYROX' \
19-'ED_GYROY' \
20-'ED_TIMESTAMP' - Timestamp of each data sample (usually real-time or internal time). \
21-'ED_ES_TIMESTAMP' - Another timestamp, which may be related to a specific event in the system. \
22-'ED_FUNC_ID' - ID of the function or data logging mode (if the device supports multiple operating modes). \
23-'ED_FUNC_VALUE' - Value related to the corresponding function or mode. \ 
24-'ED_MARKER' - Markers are added by users or devices to serve as a reference for analysis. \
25'ED_SYNC_SIGNAL' - Sync signal to connect different devices or systems. \

The EEG data is in the channels 4:17. \

III. Requirements:
1. Data Preprocessing
- Extract and load the relevant EEG data channels (4 - 17) from the provided matlab files.
- Apply preprocess, normalize, scale, or any techniques to the data if you think it neccessary for the task.

2. Feature Engineering
- Extract meaningful features from the EEG signals (e.g frequency domain features like power spectral density, and statistical features).
- Compare features across attention states to identify patterns.

3. Model Development
- Implement at least two classification models (e.g Logistic Regression, SVM, Random Forest, or Neural Networks).
- Evaluate their performance using accuracy, precision, recall, and F1 score.
- Split data into training and test sets, ensuring balanced representation of attention states.

4. Analysis and Visualization
- Visualize EEG signals and derived features to explain classification differences.
- Create confusion matrices and ROC curves for model evaluation.

5. Report
- Document data processing, feature engineering, model theory, model building, and performance evaluation.
- Discuss challenges faced and potential ways to improve accuracy.

Deliverables:
- Source code (organized and well-commented).
- A 5-minutes presentation summarizing findings.
- A detailed report (5 - 7 pages).

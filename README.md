MIDTERM - Mental Attention States Classification Using EEG DATA

I. Obbjective
- Classify mental attention states (focused, unfocused, drowsy) based on EEG signals using machine learning techniques.

II. Dataset Detail

1. Dataset source
- Dataset URL: https://www.kaggle.com/datasets/inancigdem/eeg-data-for-mental-attention-state-detection/data
- Data was acquired from EMOTIV EEG devices during 34 experiments.
- EEG data is in channels 4 to 17 of the provided Matlab files.
- Sampling frequency: 128 Hz.

2. Context
- This is a collection of 34 experiments for monitoring of attention state in human individuals using passive EEG BCI.
- Each Matlab file contains the object of the data acquired from EMOTIV device during one experiment. The raw data is contained in o.data, which is array of size {number-of-samples}x25, thus o.data(:,i) comprises one data channel. The sampling frequency is 128 Hz. The list of data channels and their numerical ids is given below per EMOTIV documentation;

1-'ED_COUNTER' - Chronological order
- Description: "Raw Contact Quality" indicates the quality of the electrode-skin contact for each sample.

2-'ED_INTERPOLATED' 
- Description: A flag indicating whether the current data point is an interpolated value.

3-'ED_RAW_CQ'
- Description: "Raw Contact Quality" indicates the quality of the electrode-skin contact for each sample.

4-'ED_AF3' - Anterior Frontal 3
- Location: Front, slightly to the left.
- Related functions: Signal processing related to decision making, planning, and attention. Linked to positive emotions and motivation.

5-'ED_F7' - Frontal 7
- Location: Left frontal lobe, near the temple.
- Related functions: Language processing, especially the ability to speak and understand. Related to negative emotions such as anxiety, sadness.

6-'ED_F3' - Frontal 
- Location: Near the middle of the forehead, to the left.
- Related functions: Decision making, planning and behavior control. Reflects focus and emotional control.

7-'ED_FC5' -  Frontocentral 5 
- Location: Between the forehead and left temple.
- Related functions: Involves the integration of sensory and motor information. Plays a role in spatial perception.

8-'ED_T7' - Temporal 7 
- Location: On the left temple.
- Related functions: Audio and language processing. Store and process memories.

9-'ED_P7' - Parietal 7
- Location: Left parietal lobe, near the back of the head.
- Related functions: Processes sensory information (touch, temperature, pain). Related to orientation and spatial awareness.

10-'ED_O1' - Occipital 1
- Location: Occipital lobe (back of head), left side.
- Related functions: Visual information processing. Relating to visual and color perception.

11-'ED_O2' - Occipital 2
- Location: Occipital lobe (back of head), right side.
- Related functions: Visual information processing. Relating to visual and color perception.

12-'ED_P8' - Parietal 8
- Location: Right parietal lobe, near the back of the head.
- Related functions: Sensory information processing and spatial perception. Often combined with ED_P7 to analyze brain symmetry.

13-'ED_T8' - Temporal 8
- Location: On the right temple.
- Related functions: Emotional processing and music. Analyze positive emotional signals.

14-'ED_FC6' - Frontocentral 6
- Location: Between the forehead and right temple.
- Related functions: Involves the integration of sensory and motor information. Plays a role in spatial perception. Relating to motor coordination.

15-'ED_F4' - Frontal 4
- Location: Near the middle of the forehead, to the right.
- Related functions: Controls behavior and emotions. Related to positive emotions and creativity.

16-'ED_F8' - Frontal 8
- Location: Right frontal lobe, near the temple.
- Related functions: Similar to ED_F7, but on the right side. Related to communication and positive emotional analysis.

17-'ED_AF4' - Anterior Frontal 4
- Location: In front of the forehead, slightly to the right.
- Related functions: Emotional regulation, decision making. Plays a role in positive cognition.

18-'ED_GYROX' 
- Description: Data from the gyroscope sensor on the X-axis.

19-'ED_GYROY' 
- Description: Data from the gyroscope sensor on the Y-axis.

20-'ED_TIMESTAMP'
- Description: Timestamp for each EEG data sample.

21-'ED_ES_TIMESTAMP'
- Description: Timestamp for events during data recording.

22-'ED_FUNC_ID'
- Description: ID of the function or operating mode of the device.

23-'ED_FUNC_VALUE'
- Description: Values related to the function or operating mode (corresponding to ED_FUNC_ID).

24-'ED_MARKER'
- Description: Markers or indicators added by users or devices for reference during analysis.

25'ED_SYNC_SIGNAL'
- Description: Synchronization signal used to connect multiple devices or systems.


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

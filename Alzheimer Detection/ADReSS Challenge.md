Tags: #Alzheimer #Psychology

>VS. Luz, F. Haider, S. de la Fuente, D. Fromm, and B. MacWhinney. Alzheimer's dementia recognition through spontaneous speech: The ADReSS challenge. In _Proceedings of INTERSPEECH 2020_, Shanghai, China, 2020. [abs](https://arxiv.org/abs/2004.06833)

- ADReSS Challenge encourages researchers to find ways to automatically detect Alzheimer's Dementia based on speech data.
- It provides a benchmark dataset containing preprocessed and balanced (in terms of age and gender) speech data for models to be trained and evaluated on.

- There are two tasks outlined in this challenge:
	- Binary Classification Task: Classify patient into two classes - AD or non-AD
	- Regression Task: Predict the MMSE score of a patient

- Other research using DementiaBank Pitt's dataset conducted multiple sessions for one subject and classify the session as AD or non-AD
	- This approach could lead to overfitting as the model could learn subject-specific features instead of learning more general features

# Dataset Description
- **Speech Recordings:** The dataset consists of speech recordings of participants who underwent the Cookie Thief Picture description task and their corresponding transcriptions
- Dataset is balanced according to age, gender, AD vs non-AD compared to DementiaBank Pitt's dataset
- **Acoustic Features** (Feature extraction done using openSMILE v2.1, emotion and affect recognition): 
	- Made up of multiple feature sets and 
	- Emobase Feature set (988 features): 
		- Mel-frequency cepstral coefficients (MFCC) voice quality, fundamental frequency (F0), F0 envelope, line spectral pairs (LSP) and intensity features with their first and second order derivatives.
	- ComParE Feature set (6373 features):
		- Energy, spectral, MFCC, and voicing related low-level descriptors (LLDs). LLDs include logarithmic harmonic-to-noise ratio, voice quality features, Viterbi smoothing for F0, spectral harmonicity and psychoacoustic spectral sharpness.
	- eGeMAPS Feature set (88 features):
		- Reduced feature set compared to above sets used to detect physiological changes in voice production
		- F0 semitone, loudness, spectral flux, MFCC, jitter, shimmer, F1, F2, F3, alpha ratio, Hammarberg index and slope V0 features
	- MRCG Functionals (768 MCRG Features):
	- Minimal feature set (13 features):
		- Duration of vocalizations, pauses, speech rate, vocalization count
- **Linguistic Features** (34 features on transcripts):
	- duration, total utterances, MLU, type-token ratio, open-closed class word ratio, percentages of 9 parts of speech

Jitter shimmmer, fnote, 

# Tasks
- Main tasks related to AD related research is described as Classification and Regression
	- Benchmark results given for those tasks using the ADReSS dataset.
- **AD Classification Task:**
	- Two step classification:
		- Segment level: Each segment is classified as either AD or non-AD
		- Subject level: Each subject is assigned a label based on majority vote from all segments
	- Result:
		- Minimal, ComParE and linguistic features show the highest accuracy
- **MMSE Prediction Task:**
	- Two step prediction (for acoustic features):
		- Segment level Regression
		- Averaging MMSE values
	- Result:
		- MRCG features chosen as baseline for regression using audio


>	https://my.clevelandclinic.org/health/diseases/9164-alzheimers-disease
>https://en.wikipedia.org/wiki/Alzheimer%27s_disease
>
# Overview
- Irreversible and progressive neurocognitive disease
- One of the main causes of dementia
- Caused by death of neurons due abnormal protein buildup between them
	- Amyloid protein buildup leads to plaque formation
	- Tau protein buildup leads to tangle formation
	- This initially leads to loss of communication between neurons then death
	- No exact cause of protein buildup discovered
- Affects people over the age of 65 (1 in 10 person over 65)
	- Early-onset AD (age 40-50) affects less than 10% of patients
	- 24 million people across the world
	- 1 in 3 over the age of 85
## Dementia
- Now called Major Neurocognitive Disorder (Major NCD) in DSM - 5
- Decline in mental function severe enough to interfere with daily life
	- Acquired deficits in mental function not developmental
	- Not part of normal aging process
- Damage to brain cells in certain areas
	- inhibited communication between those areas/cells
	- Hippocampus (responsible for memory) damaged first
- Key domains of cognitive function: 
	- executive function
	- learning and memory
	- perceptual-motor function
	- language
	- complex attention
	- social cognition
- Types of dementia
	- AD  (Alzheimer's Disease)
		- 60% - 70% cases of dementia caused by AD
	- VD (Vascular Dementia)
	- LBD (Lewy Body Dementia)
	- FD (Frontotemporal Dementia)
	- MD (Mixed Dementia)

## MCI (Mild cognitive impairment)
- Cognitive impairment that is more severe than regular symptoms of aging but not severe enough to impact day to day activities (dementia)
	- Considered a transitional stage between normal aging and dementia
- 50% of patients diagnosed with MCI go on to develop AD
- Listed as Mild Neurocognitive Disorder (Mild NCD) in DSM-5
- Types of MCI:
	- AmnesicMCI: 
## Symptoms
- Symptons grow as disease advances
- Problem with language, disorientation, mood swings, loss of motivation, self-neglect and behavioural issues
- Eventual withdrawal from family and society
- Gradual loss of bodily function leading to eventual death
# Stages

- **Preclinical AD:**
	- Symptoms don't manifest this early (asymptomatic)
	- Cognitive function is still very high
	- Last for years or decades
	- Symptoms:
		- Short term memory loss (difficulty in learning new information and remembering recent facts)
		- Inhibition of complex day to day activities
- **MCI due to AD:**
	- Transitional stage between normal ageing and dementia
	- Main symptom includes memory loss (Amnesic MCI)
		- Amnesic MCI has a greater than 90% likelihood of being associated with Alzheimer's
- **Mild dementia due to AD:**
- **Moderate dementia due to AD:**
- **Severe dementia due to AD:**
	- Almost complete loss of speech/verbal language
		- Patient generally can only communicate using single sentences, sometimes even words
		- Eventually leads to complete loss of speech
		- Patient still understands and responds to emotional signals
	- Patient shows inability to perform almost any task independently
		- Loss of muscle mass and mobility leading to patient becoming bedridden and unable to feed themselves
		- Eventual death due to external factors such as pneumonia etc.
# Diagnosis

- MMSE (Mini-Mental State Examination): set of 11 questions used to check cognitive impairment of patient
	- >25 is normal

## PET
## MRI
## CSF

# Treatment






- Main motivations of the project?
	- Detect AD early to slow down cognitive decay as much as possible using more simpler and cheaper methods
	- DL models could be much faster cheaper compared to standard diagnostic tests
	- Audio is a very convenient method to detect Alzheimers
		- Early detection of mild cognitive impairment
	- AD patients 
		- speak slower 
		- pause more often between words
		- suffer from word finding
		- suffer from word retrieval difficulties

- keywords i need to know:
	- Control Group
	- Confidence interval
	- Pvalue
	- Comorbidity
	- 

# Detection using ML

## Paper reading

- García-Gutiérrez, F., Alegret, M., Marquié, M. _et al._ Unveiling the sound of the cognitive status: Machine Learning-based speech analysis in the Alzheimer’s disease spectrum. _Alz Res Therapy_ **16**, 26 (2024). https://doi.org/10.1186/s13195-024-01394-y
	- Explore capabilities of ML techniques to discriminate between different degrees of cognitive impariment based on Spontaneous Speech

### Review Papers

- Yang, Q., Li, X., Ding, X. _et al._ Deep learning-based speech analysis for Alzheimer’s disease detection: a literature review. _Alz Res Therapy_ **14**, 186 (2022). https://doi.org/10.1186/s13195-022-01131-3
	- Traditional scale testing or imaging based diagnosis are not convenient for large scale diagnosis
		- Time consuming, labor-intensive, expensive and unfriendly to subject's experience
		- 
	- Deep learning based speech analysis and language processing techniques achieve impressive results
	- 
	- Broad categories of approaches:
		- Semantic Verbal Flulency (SVF)
			- Assess language skills, semantic memory and executive function
			- Tasks: Animal/Vegetable/Location naming
		- Spontaneous Speech (SS)
			- Speech without responding to question
			- Tasks: Conversation/interview, Day/life/dream description, recall story, picture description
		- Reading
			- Transcript reading
	- Important databases:

- Javeed, A., Dallora, A.L., Berglund, J.S. _et al._ Machine Learning for Dementia Prediction: A Systematic Review and Future Research Directions. _J Med Syst_ **47**, 17 (2023). https://doi.org/10.1007/s10916-023-01906-7
	- Analysis of ML based automatic diagnostic system for various data modalities such as images, clinical features, voice data
	- Image Modality
		- Datasets: ADNI, OASIS
		- 
	- Clinical Electronic Health Records (EHR)
		- Check for dementia status using tests:
			- Mini Mental Status Exam (MMSE)
			- Montreal Cognitive Status (MoCA)
			- Telephone Interview for Cognitive Status (TICS)
			- Brief Interview for Mental Status (BIMS)
	- Voice Modality
		- Datasets: FHS Dataset, VBSD Dataset, 
		- Chien, Y.-W., Hong, S.-Y., Cheah, W.-T., Yao, L.-H., Chang, Y.-L., Fu, L.-C.: An automatic assessment system for alzheimer’s disease based on speech using feature sequence generator and recurrent neural network. Scientific Reports **9**(1), 1–10 (2019)
		- Nishikawa, K., Akihiro, K., Hirakawa, R., Kawano, H., Nakatoh, Y.: Machine learning model for discrimination of mild dementia patients using acoustic features. Cognitive Robotics (2021)
		- Liu, L., Zhao, S., Chen, H., Wang, A.: A new machine learning method for identifying alzheimer’s disease. Simulation Modelling Practice and Theory **99**, 102023 (2020)
		- Searle, T., Ibrahim, Z., Dobson, R.: Comparing natural language processing techniques for alzheimer’s dementia prediction in spontaneous speech. arXiv preprint [arXiv:2006.07358](http://arxiv.org/abs/2006.07358) (2020)
		- Zhu, Y., Tran, B., Liang, X., Batsis, J.A., Roth, R.M.: Towards interpretability of speech pause in dementia detection using adversarial learning. arXiv preprint [arXiv:2111.07454](http://arxiv.org/abs/2111.07454) (2021)
		- Xue, C., Karjadi, C., Paschalidis, I.C., Au, R., Kolachalama, V.B.: Detection of dementia on voice recordings using deep learning: a framingham heart study. Alzheimer’s research & therapy **13**(1), 1–15 (2021)
		- 
		- Edwards, E., Dognin, C., Bollepalli, B., Singh, M.K., Analytics, V.: Multiscale system for alzheimer’s dementia recognition through spontaneous speech. In: INTERSPEECH, pp. 2197–2201 (2020)
		- Kumar, Y., Maheshwari, P., Joshi, S., Baths, V.: Ml-based analysis to identify speech features relevant in predicting alzheimer’s disease. arXiv preprint [arXiv:2110.13023](http://arxiv.org/abs/2110.13023) (2021)
		- SOTA (88% accuracy on DementiaBank): Sarawgi, U., Zulfikar, W., Soliman, N., Maes, P.: Multimodal inductive transfer learning for detection of alzheimer’s dementia and its severity. arXiv preprint [arXiv:2009.00700](http://arxiv.org/abs/2009.00700) (2020)
	- Handling Bias
		- Imbalance classes in dataset lead to bias in models
		- Bias in models measures using sensitivity and specificity
		- Overcome by oversampling or undersampling the data
			- Random oversampling
			- Synthetic minority oversampling technique
	- SVM most often used for binary classifier for dementia prediction
		- RF in second, CNN in third
	- Future Directions:
		- Publicly available datasets are modest in size
		- Using image modality gave high accuracy for large datasets, whereas voice modality gave high accuracy for smaller datasets
			- Recent trend in working on voice modality
		- Unsupervised learning underutilized
			- While not as accurate, more expressive (what does this mean?)
		- Exploring and exploiting multimodality
- Vigo I, Coelho L, Reis S. Speech- and Language-Based Classification of Alzheimer's Disease: A Systematic Review. Bioengineering (Basel). 2022 Jan 11;9(1):27. doi: https://doi.org/10.3390/bioengineering9010027
- Almatrafi, S., Abbas, Q. & Ibrahim, M.E.A. A systematic literature review of machine learning approaches for class-wise recognition of Alzheimer’s disease using neuroimaging-based brain disorder analysis. _Multimed Tools Appl_ (2024). https://doi.org/10.1007/s11042-024-19104-z
- Alsubaie MG, Luo S, Shaukat K. Alzheimer’s Disease Detection Using Deep Learning on Neuroimaging: A Systematic Review. _Machine Learning and Knowledge Extraction_. 2024; 6(1):464-505. https://doi.org/10.3390/make6010024
### Audio/Speech Based

- What is the broad difference between audio vs speech based methods?
	- Can we find speech data from audio?
	- What does speech data even look like? 
		- How do you account for pauses, gaps, speech patterns?

- Alzheimer's Dementia Recognition through Spontaneous Speech: The ADReSS Challenge https://arxiv.org/abs/2004.06833 (2020)
	- Describing the ADReSS Dataset/benchmark


- The Effect of Heterogeneous Data for Alzheimer's Disease Detection from Speech https://arxiv.org/abs/1811.12254v1 (2018)
	- https://github.com/ychnlgy/Chebyshev-Lagrange
- Multi-Modal Detection of Alzheimer's Disease from Speech and Text https://arxiv.org/abs/2012.00096 (2020)
- MRI-based Multi-task Decoupling Learning for Alzheimer's Disease Detection and MMSE Score Prediction: A Multi-site Validation https://arxiv.org/abs/2204.01708v3 (2022)
	- https://arxiv.org/abs/2204.01708v3
- Exploiting prompt learning with pre-trained language models for Alzheimer's Disease detection https://arxiv.org/abs/2210.16539v2 (2022)
- SpeechFormer++: A Hierarchical Efficient Framework for Paralinguistic Speech Processing https://arxiv.org/abs/2302.14638v1 (2023)
	- https://github.com/happycolor/speechformer2
- Exploring Multimodal Approaches for Alzheimer's Disease Detection Using Patient Speech Transcript and Audio Data https://arxiv.org/abs/2307.02514v1 (2023)
	- https://github.com/shui-dun/multimodal_ad
	- 
- Xue, C., Karjadi, C., Paschalidis, I.C. _et al._ Detection of dementia on voice recordings using deep learning: a Framingham Heart Study. _Alz Res Therapy_ **13**, 146 (2021). https://doi.org/10.1186/s13195-021-00888-3
- A Deep Learning-Based Multimodal Architecture to predict Signs of Dementia https://www.sciencedirect.com/science/article/pii/S0925231223005362#ab005
- Loukas Ilias, Dimitris Askounis, John Psarras, Detecting dementia from speech and transcripts using transformers, Computer Speech & Language, Volume 79, 2023, 101485, ISSN 0885-2308, https://doi.org/10.1016/j.csl.2023.101485
- Priyadarshinee P, Clarke CJ, Melechovsky J, Lin CMY, B. T. B, Chen J-M. Alzheimer’s Dementia Speech (Audio vs. Text): Multi-Modal Machine Learning at High vs. Low Resolution. _Applied Sciences_. 2023; 13(7):4244. https://doi.org/10.3390/app13074244
- Jahan, Z., Khan, S.B. & Saraee, M. Early dementia detection with speech analysis and machine learning techniques. _Discov Sustain_ **5**, 65 (2024). https://doi.org/10.1007/s43621-024-00217-2
	- Research Gaps:
		- 

- Y. F. Khan, B. Kaushik, M. K. I. Rahmani and M. E. Ahmed, "Stacked Deep Dense Neural Network Model to Predict Alzheimer’s Dementia Using Audio Transcript Data," in _IEEE Access_, vol. 10, pp. 32750-32765, 2022, doi: https://doi.org/10.1109/ACCESS.2022.3161749
	- Model: CNN + BiLSTM (Stacked Deep Dense NN)
	- Dataset: DementiaBank

- Park, C. Y., Kim, M., Shim, Y., Ryoo, N., Choi, H., Jeong, H. T., Yun, G., Lee, H., Kim, H., Kim, S., & Youn, Y. C. (2024). Harnessing the Power of Voice: A Deep Neural Network Model for Alzheimer's Disease Detection. _Dementia and neurocognitive disorders_, https://doi.org/10.12779/dnd.2024.23.1.1

- S. Luz, F. Haider, D. Fromm, I. Lazarou, I. Kompatsiaris and B. MacWhinney, "An Overview of the ADReSS-M Signal Processing Grand Challenge on Multilingual Alzheimer's Dementia Recognition Through Spontaneous Speech," in _IEEE Open Journal of Signal Processing_, https://doi.org/10.1109/OJSP.2024.3378595

### Journals referred
- Alzheimer's review and therapy
	- Impact Factor (Web of Science Group): 6.982
	- H Index: 77
	- Impact Factor (Scopus): 7.77
- Applied Sciences (Switzerland)
	- Impact Factor (Web of Science Group): NA
	- H Index: 75
	- Impact Factor (Scopus): 3.143
- IEEE Access
	- Impact Factor (Web of Science Group): 3.367
	- H Index: 158
	- Impact Factor (Scopus): 4.342
- Bioengineering (Basel)
	- Impact Factor (Web of Science Group): NA
	- H Index: 37
	- Impact Factor (Scopus): 4.864
- Computer Speech & Language
	- Impact Factor (Web of Science Group): 1.899
	- H Index: 72
	- Impact Factor (Scopus): 4.479
## Datasets

#### Image based
- OASIS (Open Access Series of Imaging Studies)
- ADNI (Alzheimer's Disease Neuroimaging Initiative)
#### Audio based
- DementiaBank (Transcript with media)
	- Specifically the pitt dataset
- PGA-Oreka
- ADReSS

### Models
- WavLM
# Paper 1 from Paperswithcode

>[Exploring Multimodal Approaches for Alzheimer's Disease Detection Using Patient Speech Transcript and Audio Data](https://scholar.google.com.hk/scholar?oi=bibs&cluster=9695613838314695061&btnI=1&hl=zh-CN)H Cai, X Huang, Z Liu, W Liao, H Dai, Z Wu, D Zhu… - arXiv preprint arXiv:2307.02514, 2023

- Speech patterns of people suffering from early stages of AD show characteristics such as frequent silence, incoherence, word retrieval difficulty and repetition
- 
## Methods
### GNN based method
- Takes raw text as input and embeds each token
- Graph Construction:
	- Dependency graph: relation between words to describe text structure
	- Dynamic graph: 
	- Fused graph
- 
### Data Augmenter + GNN based method
- Data augmentation is used to generate modified versions of exisiting data
	- Used to address issues of limited datasets by artificially increasing size of dataset
	- Can increase diversity of dataset and reduce risk of overfitting
- Synonym Replacement: 
- Counter-fitting Embedding Replacement:
- Masked Language Model Augnmentation:
- Random Sequence Deletion:
### Multimodal (Audio + Speech) method
### CLIPPO-like method

## Research Gap
- Implementing facial features of the patients to improve detection
- Data augmentation methods to better simulate language features
	- Current methods don't show good results

# Paper 2 from biomedcentral (part of springer nature)

>García-Gutiérrez, F., Alegret, M., Marquié, M. _et al._ Unveiling the sound of the cognitive status: Machine Learning-based speech analysis in the Alzheimer’s disease spectrum. _Alz Res Therapy_ **16**, 26 (2024). https://doi.org/10.1186/s13195-024-01394-y

- Patients start cognitive decline before the clinical symptoms for AD/Dementia start manifesting
	- Language deficits start occurring in patients before they enter Dementia stage
	- Identifying those can be used to detect early stages of MCI in patients

## Cognitive Composites and Domains
### ### Cognitive Domains
- Main cognitive domains typically examined in AD:
	- Memory
	- Attention
	- Visuospatial functions
	- Executive functions
	- Language	
- The linguistic ability of a patient measured using SS is correlated with cognitive domains 
	- memory
	- attention
	- executive functions
### Cognitive Scores
- Composite scores from various neuropsychological tests performed on patients are calculated
	- Scores summarize the results of those tests and help reduce redundancy between variables
	- They give a comprehensive overview of a patients status in various cognitive domains
## Methodology
- Main problems addressed:
	- Classification model to differentiate between clinical phenotypes based on analysis of SS test:
		- Preserved cognition/Subjective cognitive decline (SCD)
		- MCI
		- AD
	- Predict cognitive scores for various cognitive domains using information obtained from analysis of SS test
- Acoustic features (eGeMAPS feature set) obtained from SS used as input for both models
## Results
- SCD - Highest scores for domains
- MCI - Intermediate scores
- ADD - Lowest scores
## Research Gaps
- More diverse parameters for SS can be used for better performance
- 
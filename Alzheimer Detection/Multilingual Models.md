# Motivation
- The small size of AD datasets proves to be a big hurdle in training models to detect AD early in patients. 
- There are a few methods that can be used to overcome this issue, for example: Data Augmentation
- Another method that could be used to augment the limited dataset would be to augment it with data in another language
	- For example: To train a model to detect AD in patients in India we might collect data in Hindi. But collecting data is a time consuming process and very expensive. To overcome the limitations of a Hindi AD dataset we might augment it with the DementiaBank Pitts dataset
# Issues
- While augmenting a dataset in one language with another we need to find a set of audio features that can predict AD common to both languages
- This is because there are variations in phonology and prosody between different languages that might give different results for the same set of acoustic features
- 
# Approaches

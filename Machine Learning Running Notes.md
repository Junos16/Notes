# Linear Models
Why use squared error instead of modulus?
Why normalize independent features?
	For small ranges of features the weights are large and vice versa
	Difference in range make comparing weights challenging (can't compare corresponding impact of features)
	Normalization makes the weights more comparable
What is cross entropy

## Gradient Descent
What is learning rate
What is bias?
What are hyperparameters?
### Optimizers
SGD: Proportional to gradient
Momentum: Use past grad values to better assess slope and make larger jumps
	Cause overshooting
NAG:
RMSProp: Speeds up convergence in cases where one parameters grad dominates
	wont spend time optimizing one parameter then the next, would do both simultaneously
Adam: 

# Neural Networks
When to use neural networks instead of linear models?
	Main reason being cost benefit analysis
	Non-linear models capture linear relationships as well
# Computer Vision
Image Filtering

- Chomsky Hierarchy is a way to classify formal languages and grammars based on their expressive powers
- We can use this hierarchy to compare the relative computability power of a model of computation
	- The more complex the language that a model can recognize the more powerful it is
	- ***Example:*** A Push-Down Automata can recognize all regular languages 
# Regular Language/Grammar (Type-3)
- ***Regular Language:*** The set of regular languages over the alphabet $\Sigma$ is defined recursively as follows:
	1. $\epsilon$ and the empty language are regular languages
	2. $\forall x\in\Sigma \{x\}$ is regular
	3. $A$ is regular $\implies$ $A^{*}$ is regular
	4. If $A$ and $B$ are regular languages $\implies A\cup B$ and $A\cdot B$ are regular
	5. No other language over $\Sigma$ are regular
- ***Regular Grammar:*** 
# Context-Free Language/Grammar (Type-2)
- ***Context-Free Language:*** The set of context-free languages over the alphabet $\Sigma$ is defined recursively as follows:
	1. 
- ***Context-Free Grammar:*** A context-free grammar $G$ is the tuple: $G=(V,\Sigma,R,S)$, where
	1. 
## Context-Free Language
## Context-Free Grammar
# Context-Sensitive Language/Grammar (Type-1)
## Context-Sensitive Language
## Context-Sensitive Grammar
# Recursively Enumerable Language/Grammar (Type-0)
## Recursively Enumerable Language
## Recursively Enumerable Grammar

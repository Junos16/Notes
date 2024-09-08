For some reason a lot of textbooks think its cool to not define half of the terms they are using to prove theorems lmao

It would be nice to fix that issue and have a repository for all the definitions and theorems stated properly
# Basics
- Primitives: 
	- Symbols: Some object, sets in the case of pure set theory
	- Alphabets: A set containing symbols
- **String:** Ordered n-tuple of 
- **Grammar:** A grammar $G$ is a 4-tuple $G=(V,T,S,P)$ where
	- $V$ is a finite set of symbols called **Variables**
	- $T$ is a finite set of symbols called **Terminal Symbols**
	- $S\in V$ is a special symbol called the **Start Symbol**
	- $P$ is a finite set of **Productions**
		- Depending on the specific use case we can later define the domain and range of the function as some combination of $V$, $T$ and $S$
# Type3
## DFA
- **DFA:** A DFA is a 5-tuple $M=(Q,\Sigma,\delta,q_{0},F)$ where
	- $Q$ is a finite set of internal states
	- $\Sigma$ is a finite set of symbols called input alphabet
	- $\delta:Q\times\Sigma\rightarrow Q$ is a total function called the transition function
	- $q_{0}\in Q$ is the initial state
	- $F\subseteq Q$ is a set of final states
- **Extended Transition Function:** $\delta^{*}:Q\times\Sigma^{*}\rightarrow Q$ is a function for the DFA $M$ such that $\forall q\in Q,w\in\Sigma^{*},a\in\Sigma$
	- $\delta^{*}(q,\epsilon)=q$
	- $\delta^{*}(q,wa)=\delta(\delta^{*}(q,w),a)$
- **Acceptance of String by DFA:** A string $w$ is accepted by DFA $M\iff\delta^{*}(q_{0},w)\in F$
- **Language recognized by DFA:** A language $\Sigma^{*}$ is recognized by DFA $M\iff\forall w\in\Sigma$* $w$ is accepted by $M$
	- $L(M):=\{w\in\Sigma^{*}:\delta^{*}(q_{0},w)\in F\}$ is the language of the DFA $M$
- **Rejection of String by DFA:** A string $w$ is rejected by DFA $M\iff \delta^{*}(q_{0},w)\notin F$ 
	- $\overline{L(M)}:=\{w\in\Sigma^{*}:\delta^{*}(q_{0},w)\notin F\}$ is the complement of the language of the DFA $M$
- **Transition Graph:**
- **Proposition (Existence of walk in graph):**
- **Regular Language:** A language $L$ is regular iff there exists DFA $M$ such that $L=L(M)$
## Minimal DFA
## NFA
- **NFA:** An NFA is a 5-tuple $M=(Q,\Sigma,\delta,q_{0},F)$ where
	- $Q$ is a finite set of internal states
	- $\Sigma$ is a finite set of symbols called input alphabet
	- $\delta:Q\times(\Sigma\cup\{\epsilon\})\rightarrow 2^{Q}$ is a total function called the transition function
	- $q_{0}\in Q$ is the initial state
	- $F\subseteq Q$ is a set of final states
NEED TO EDIT THE FOLLOWING!!!!!!!!!!
- **Extended Transition Function:** $\delta^{*}:Q\times\Sigma^{*}\rightarrow Q$ is a function for the DFA $M$ such that $\forall q\in Q,w\in\Sigma^{*},a\in\Sigma$
	- $\delta^{*}(q,\epsilon)=q$
	- $\delta^{*}(q,wa)=\delta(\delta^{*}(q,w),a)$
- **Acceptance of String by DFA:** A string $w$ is accepted by DFA $M\iff\delta^{*}(q_{0},w)\in F$
- **Language accepted by DFA:** A language $\Sigma^{*}$ is accepted by DFA $M\iff\forall w\in\Sigma$* $w$ is accepted by $M$
	- $L(M):=\{w\in\Sigma^{*}:\delta^{*}(q_{0},w)\in F\}$ is the language of the DFA M
- **Nonacceptance of String by DFA:** A string $w$ is not accepted by DFA $M\iff \delta^{*}(q_{0},w)\notin F$ 
	- $\overline{L(M)}:=\{w\in\Sigma^{*}:\delta^{*}(q_{0},w)\in F\}$ is the complement of the language of the DFA M
- **Transition Graph:**
!!!!!!
- **Theorem (Equivalence in power of NFA and DFA):** $\forall$ NFA $M_{1}\space\exists$ DFA $M_{2}\ni L(M_{1})=L(M_{2})$
## regex
- **Regex:** A regular expression is a string. Let $\Sigma$ be a given alphabet. Then
	- $\emptyset,\epsilon$ and $a\in\Sigma$ are all regular expressions (primitive regular expressions)
	- If $r_{1}$ and $r_{2}$ are regular expressions then $r_{1}+r_{2},r_{1}\cdot r_{2},r_{1}^{*}$ and $(r_{1})$ are also regular expressions
- **Language of the regex:** For a regex string $r$ we define the language recognized by it following rules:
	- $L(\emptyset)=\emptyset$
	- $L(\epsilon)=\{\epsilon\}$
	- $\forall a\in\Sigma L(a)={a}$
	- If $r_{1}$ and $r_{2}$ are two regular expressions then
		- $L(r_{1}+r_{2})=L(r_{1})\cup L(r_{2})$
		- $L(r_{1}\cdot r_{2})=L(r_{1})L(r_{2})$
		- $L((r_{1}))=L(r_{1})$
		- $L(r_{1}^{*})=(L(r_{1}))^{*}$
- **Proposition (NFA for regex):** $\forall$ regex $r\space\exists$ an NFA $M\ni L(M) = L(r)$ 
- **Proposition:** For a regular language $L\space\exists$ regex $r\ni L=L(r)$
## Regular Grammar
- **Right Linear Grammar:** A grammar $G$ is right-linear if $\forall p\in P\space domain(p)=V\cup{S},\space range(p)=$  

## Closure Properties of RegLang
## Non-Regular Lang
Pigeonhole Proof
Pumping Lemma
## Type 2
## Push-Down Automata
- **Non-Deterministic Push-Down Automata:** An NPDA is a 7-tuple $M=(Q,\Sigma,\Gamma,\delta,q_{0},F)$ where
	- $Q$ is a finite set of internal states of the control unit
	- $\Sigma$ is the input alphabet
	- $\Gamma$ is a finite set of symbols called the stack alphabet
	- $\delta:Q\times(\Sigma\cup\{\epsilon\})\times(\Gamma\cup\{\epsilon\})\rightarrow2^{Q\times\Gamma\cup\{\epsilon\}}$ is the transition function
	- $q_{0}\in Q$ is the initial state of the control unit
	- $z\in\Gamma$ is the stack start symbol
	- $F\subseteq Q$ is the set of final states
NEED TO EDIT THE FOLLOWING!!!!!!!!!!
- **Extended Transition Function:** $\delta^{*}:Q\times\Sigma^{*}\rightarrow Q$ is a function for the DFA $M$ such that $\forall q\in Q,w\in\Sigma^{*},a\in\Sigma$
	- $\delta^{*}(q,\epsilon)=q$
	- $\delta^{*}(q,wa)=\delta(\delta^{*}(q,w),a)$
- **Acceptance of String by DFA:** A string $w$ is accepted by DFA $M\iff\delta^{*}(q_{0},w)\in F$
- **Language accepted by DFA:** A language $\Sigma^{*}$ is accepted by DFA $M\iff\forall w\in\Sigma$* $w$ is accepted by $M$
	- $L(M):=\{w\in\Sigma^{*}:\delta^{*}(q_{0},w)\in F\}$ is the language of the DFA M
- **Nonacceptance of String by DFA:** A string $w$ is not accepted by DFA $M\iff \delta^{*}(q_{0},w)\notin F$ 
	- $\overline{L(M)}:=\{w\in\Sigma^{*}:\delta^{*}(q_{0},w)\in F\}$ is the complement of the language of the DFA M
- **Transition Graph:**

!!!!!!!
- **Context-Free Language:** A language $L$ is context-free iff there exists NPDA $M$ such that $L=L(M)$
- **Deterministic Context-Free Language:** A language $L$ is deterministic context-free iff there exists DPDA $M$ such that $L=L(M)$
## Context-Free Grammar
- **Context-Free Grammar**

## Context-Free Languages
## Turing Machine
- ***Turing Machine:*** A Turing Machine is a 7-tuple $M=(Q,\Sigma,\Gamma,\delta,q_{0},\square,F)$ where
	- $Q$ is the set of internal states
	- $\Gamma$ is a finite set of symbols called the tape alphabet
	- $\square\in\Gamma$ is a special symbol called the blank symbol
	- $\Sigma$ is the input alphabet where $\Sigma\subseteq\Gamma-\{\square\}$
	- $\delta:Q\times\Gamma\rightharpoonup Q\times\Gamma\times\{L,R\}$ is the transition function (a partial function since the function is undefined if the symbol is in $\Gamma$ and not in $\Sigma$)
	- $q_{0}\in Q$ is the initial state
	- $F\subseteq Q$ is the set of final states i.e. $\delta$ is undefined for $F$
- ***Configuration of Turing Machine:*** For a Turing Machine $M$ the string $a_{1}a_{2}...a_{k-1}q_{1}a_{k}a_{k+1}...a_{n-1}a_{n}$ where $a_{i}\in\Gamma$ and $q_{1}\in Q$ is its configuration
	- ***Consecutive Configurations of a Turing Machine:*** For a Turing Machine $M$ the ordered n-tuple of configurations $(c_0,c_1,...,c_n)$ is considered consecutive $\iff\forall i\in[0,n-1]$ if $c_{i}:=x_{i,1}q_{i}a_{i}x_{i,2}$ and $c_{i+1}:=x_{i+1,1}a_{i+1},q_{i+1},x_{i+1,2}$ then $\delta(q_{i},a_{i})=(q_{i+1},a_{i+1},R)$ or if $c_{i}:=x_{i,1}q_{i}a_{i}x_{i,2}$ and $c_{i+1}:=x_{i+1,1}q_{i+1},a_{i+1},x_{i+1,2}$ then $\delta(q_{i},a_{i})=(q_{i+1},a_{i+1},L)$
		- If it is an ordered pair then we use the shorthand $c_{i}\vdash c_{i+1}$ else we use the shorthand $c_{i}\vdash^{*} c_{i+1}$

- ***Halting of Turing Machine:*** A Turing Machine $M$ is said to halt from some initial configuration $x_{1}q_{1}x_{2}\iff\exists x_{1}q_{1}x_{2}\vdash^{*}y_{1}q_{2}ay_{2}\ni\delta(q_{2},a)$ is undefined. $M$ is said to have halted at $y_{1}q_{2}ay_{2}$ 
- ***Language decided by TM:*** A language $\Sigma^{*}$ is decided by TM $M\iff\forall w \in\Sigma^{*}$ $M$ halts from initial configuration $q_{0}w$
- ***Looping of Turing Machine:*** A Turing Machine $M$ is said to loop from some initial configuration $x_{1}q_{1}x_{2}\iff\forall x_{1}q_{1}x_{2}\vdash^{*}y_{1}q_{2}ay_{2}\space\delta(q_{2},a)$ is defined. The shorthand $x_{1}q_{1}x_{2}\vdash^{*}\infty$ is used to state that $M$ loops for initial configuration $x_{1}q_{1}x_{2}$
- ***Acceptance of String by a Turing Machine:*** A string $w\in\Sigma^{+}$ is accepted by a TM $M \iff \exists q_{0}w\vdash^{*}x_{1}q_{f}ax_{2}\ni\delta(q_{f},a)\text{ is undefined }\land q_{f}\in F$ ($M$ halts at a final state for the given input) where $x_{1},x_{2}\in\Gamma^{*},a\in\Gamma$
- ***Language accepted/recognized by TM:*** A language $\Sigma^{*}$ is accepted/recognized by TM $M\iff\forall w\in\Sigma^{*}$ $w$ is accepted by $M$
	- $L(M):=\{w\in\Sigma^{*}:\exists q_{0}w\vdash^{*}x_{1}q_{f}ax_{2}\ni\delta(q_{f},a)\text{ is undefined}\land q_{f}\in F;x_{1},x_{2}\in\Gamma^{*},a\in\Gamma\}$ is the language of the DFA M 
- ***Rejection of String by a Turing Machine:*** A string $w\in\Sigma^{*}$ is rejected by a TM $M\iff\forall w\in\Sigma^{*}\forall q_{0}w\vdash^{*}x_{1}q_{f}ax_{2}(\delta(q_{f},a)\text{ is defined }\lor q_{f}\notin F)$ ($M$ loops for given input or halts at a non-final state) where $x_{1},x_{2}\in\Gamma^{*},a\in\Gamma$
	- $\overline{L(M)}:=\{w\in\Sigma^{*}:\forall q_{0}w\vdash^{*}x_{1}q_{f}ax_{2}(\delta(q_{f},a)\text{ is defined }\lor q_{f}\notin F);x_{1},x_{2}\in\Gamma^{*},a\in\Gamma\}$ is the complement of the language of the Turing Machine $M$
- ***Turing-Computable Functions:*** A function $f:X\rightarrow Y$ is Turing-Computable $\iff\exists$ Turing Machine $M$ such that $\forall w\in X\exists q_{0}w\vdash^{*}xq_{f}f(w)\ni q_{f}\in F$
- ***Algorithm:*** An Algorithm for the Turing-Computable function $f:X\rightarrow Y$ is a Turing Machine such that $\forall w\in X\exists q_{0}w\vdash^{*}xq_{f}f(w)\ni\delta(q_{f},f(w))\text{ is undefined }\land q_{f}\in F$
- ***Equivalence of Classes of Automata:*** Two classes of Automata $C_{1}$ and $C_{2}$ are considered equal in power $\iff\forall M_{1}\in C_{1}\exists M_{2}\in C_{2}\ni L(M_{1})=L(M_{2})$
	- ***Equivalence of Automata:*** Two Automata $M_{1}$ and $M_{2}$ are considered equal in power $\iff L(M_{1})=L(M_{2})$
- **Proof of Equivalence using Simulation:**
- ***Recursively Enumerable Languages:*** A Language $L\subseteq\Sigma^{*}$ is recursively enumerable  $\iff\exists$ Turing Machine $M\ni\forall w\in L\space w$ is accepted by $M$  
- ***Recursive Languages:*** A Language $L\subseteq\Sigma^{*}$ is recursive $\iff\exists$ Turing Machine $M\ni\forall w\in L\space w$ is accepted by $M$ and $\forall w\in\Sigma^{*}\space M$ halts for $w$
	- More specific than recursively enumerable languages, on top of accepting language it halts for complement of language
- 
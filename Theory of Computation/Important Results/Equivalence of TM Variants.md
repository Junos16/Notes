- There are some variants of TMs that seem to improve it but it can be shown that all of them are equivalent in power in their ability to recognize languages
- To show that a TM variant is just as powerful as a basic TM I would need to show that there exists a TM that accepts the exact same language as the variant
- The standard way to do that is to construct a basic TM that would simulate the transitions of the variant
	- For every transition of the variant there would be a 
# Minor Variants of Turing Machines
## Turing Machine with Stay Option
>***Theorem (TM with stay option):*** The class of all TM with a stay option is equivalent to the class of all standard TMs

Proof (Formal):

Proof (By Church-Turing Thesis):

## Turing Machine with Semi-Infinite Tape
>***Theorem (TM with semi-infinite tape):*** The class of all TM with a semi-infinite tape is equivalent to the class of all standard TMs (tape is infinite in both directions)

Proof:

## Off-Line Turing Machine
>***Theorem (Off-Line TM):*** The class of all Off-Line TM is equivalent to the class of all standard TMs

Proof:
# Turing Machines with more Complex Storage
## Multi-Tape Turing Machine
>***Theorem (Multi-tape TM):*** The class of all Multi-tape TM is equivalent to the class of all standard TMs

Proof (By Church-Turing Thesis):
## Multidimensional Turing Machine
>***Theorem (Multidimensional TM):*** The class of all Multidimensional TM is equivalent to the class of all standard TMs

# More Complex Variants
## Non-Deterministic Turing Machine
>***Theorem (Non-Deterministic TM):*** The class of all Non-Deterministic TM is equivalent to the class of all standard TMs

## Enumerator
> For all enumerators, there is an equivalent single-tape TM

## Universal Turing Machine
# GreedySortingReversals

# Description
GreedySortingReversals is a Python implementation of the greedy sorting algorithm used to sort signed permutations into the identity permutation using reversal operations. This approach is fundamental in comparative genomics, particularly in analyzing genome rearrangements between species.

The algorithm iteratively searches for out-of-place elements and reverses segments of the permutation to bring them closer to their correct position, flipping signs when necessary. Each reversal step is stored for later analysis.

# Features
* Sorts signed permutations using greedy strategy.
* Tracks and returns the full sequence of reversal steps.
* Efficiently handles large permutations.
* Returns number of steps (reversals) needed to sort the permutation.

# Function
```
GreedySortingReversals(permutation)
```

# Purpose:
* Finds the minimum sequence of signed reversals needed to transform a given permutation into the identity permutation.

# Parameters
* permutation (list[int]): A list of integers representing a signed permutation (e.g., [+3, -4, +1, +5, -2]).

# Returns
* list[list[int]]: A list of permutations representing each intermediate step in the reversal process.

# Example
```
permutation = list(range(100, 0, -1))  # [+100, +99, ..., +2, +1]
reversals = GreedySortingReversals(permutation)

print("Number of reversals needed:", len(reversals))
```

# Output
* Number of reversals needed: 100

# Applications
* Comparative Genomics: Studying gene order changes between species.
* Genome Rearrangement: Measuring evolutionary distance in genome architecture.
* Bioinformatics Education: Teaching algorithms related to sequence and genome analysis.

# Requirements
* Python 3.x
* No external libraries required.

# License
This project is licensed under the MIT License. See the LICENSE file for details.







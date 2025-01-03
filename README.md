# R Subsetting Error: Logical Vector Length Mismatch

This repository demonstrates a common yet easily overlooked error in R: attempting to subset a data frame using a logical vector whose length doesn't match the number of rows in the data frame.  This can lead to unexpected results and hard-to-debug errors.

## The Bug
The `bug.R` file contains code that attempts to subset a data frame using a logical vector that is shorter than the number of rows in the data frame. This results in a silent error; R silently recycles the shorter vector to match the length of the data frame, which frequently leads to incorrect subsetting.

## The Solution
The `bugSolution.R` file demonstrates the correct way to subset a data frame, ensuring that the logical vector's length always matches the data frame's row count.  It also includes error handling to prevent this issue from occurring.

## How to Reproduce
1. Clone this repository.
2. Open `bug.R` and run the code. Observe the unexpected results.
3. Open `bugSolution.R` and run the code to see the corrected behavior.
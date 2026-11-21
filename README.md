# Reflection – AI Number Program Lab

##  Student Name:
Sky Rezac

##  GitHub Repository Link:
https://github.com/srezac115/cmsc115_unit8_lab2.git

## Iteration 1

What the AI code does:
- The initial implementation sums the elements in the array rather than finding the largest value or handling edge cases like null arrays.

Tests passed/failed:
- Tests expecting the max value in an array fail because summing values does not return the largest integer.

What surprised you:
- Without the full goal in the first prompt, the AI made a resonable guess that didn't match the actual problem requirements.

Commit message:
- Iteration 1: AI-generated implementation

---

## Iteration 2

What changed:
- Replaced the summation logic with a loop starting at index 1 that compares each element against max and updates it whenever a larger value is found.

What improved:
- Standard non empty arrays now properly return the largest integer in the array instead of the sum.

What still failed and why:
- Passing an empty array still fails with an index out of bounds error because values[0] is accessed before checking whether any elements exist.

Commit message:
- Iteration 2: largest value implementation

---

## Iteration 3

Final behavior:
- Returns Integer.MIN_VALUE if the array is null, and otherwise iterates through values to return the largest integer.

What was fixed:
- Added a guard check before indexing values[0] so empty arrays no longer throw an out of bounds exception and all JUnit tests pass.

What you learned:
- Refining prompts and pairing AI-generated code with JUnit tests quickly exposes edge case assumptions and leads to more reliable code.

Commit message:
- Iteration 3: final version passing all tests

---

## Final Reflection

It completed the overall reflection summary tying together the three iterative code updates, JUnit test verifications, Git commit history, and final submission for zyBooks. Running the JUnit tests after each iteration showed what the code actually handled versus where it broke. It confirmed that iteration 1's logic didn't match the goal and iteration 2 failed on empty arrays, and verifying iteration 3 made all test cases pass. Version control helped me understand how a program evolves step by step across checkpoints. It made it clear why keeping a clean, ordered history matters when refining code.

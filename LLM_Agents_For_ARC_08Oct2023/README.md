# ARC-Challenge-Multiple-Expert-Agents

## Code_Notebook.ipynb
- Run the Jupyter Notebook for the code.
- An OpenAI API key is required to use the GPT-4 API.

## ARC Tasks.zip
- For the ARC Tasks.zip, download and unzip it.
- When opened, it contains listing.html, which can open the folders in a directory for easy viewing.
- The folders are:
  1. solved (contains 50 solved ARC tasks)
  2. train_pass_but_test_failed (contains 3 ARC tasks whose programs solve the training tasks but not the test task)
  3. unsolved (contains 58 unsolved ARC tasks)
- Each .html file contains the training and test input and outputs, and GPT's output (if code compiles).
- GPT's test output is only provided if it passes all the training inputs.
- There can be up to 2 iterations for GPT to use environmental feedback to refine the code.
- If there is a compile error, we can go up to 3 iterations.



# ARC-Challenge

This contains a series of Jupyter notebooks (with date in the file name), to document the progress I have made at getting GPT4 to solve ARC.

Papers:
- https://arxiv.org/abs/2306.03553 - An Approach to Solving the Abstraction and Reasoning Corpus (ARC) Challenge: My Lab42 ARC Essay Challenge submission, based primarily on my initial experiments documented in arc_challenge_basic.ipynb
- I have more progress so far, and will write a follow-up paper shortly, after I finish experimenting on the ARC training set. The new approach involves:
  * Full end-to-end pipeline without human intervention
  * Sample input/output pairs to language description
  * Language description to list of functions via function grounding in human priors
  * Conditional function execution using if statements to check on conditions (I call this the Instructions Code Format)
  * Better processing of input grid via objects
  * Reflection-like pathway using environment feedback multiple times as in Voyager / Ghost in the Minecraft
  * Broad to specific grounding via efficient prompting

Videos:
- https://www.youtube.com/watch?v=vt2yG1da8Fg - Explanation of my initial experiments documented in arc_challenge_basic.ipynb 

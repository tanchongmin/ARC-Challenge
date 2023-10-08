# ARC-Challenge

## Refined Update (8 Oct):
Solves 50 out of 111 training set problems! No change to earlier 22 Jul update. Added a more refined UI to go through the .html files for the 111 problems. Jupyter Notebook included inside the folder "LLM_Expert_Agents_For_ARC_08Oct2023"

Based on the latest paper, intending to add more functions and to refine the agents to improve performance, stay tuned!

## 22 Jul:
Solves 50 out of 111 training set problems! Uses object and pixel abstraction spaces and helper functions to ground input-output relation!
- Added ARC_Challenge_22Jul2023.ipynb : Latest iteration of GPT4 API to automate solving ARC Challenge - Note it can get expensive, running one iterative feedback loop cycle for one task costs about 30-40 cents.
- Added ARC_Training_220723 folder to showcase results from this Jupyter Notebook on 111 training set problems that have <3k context length. This number caters for the iterative feedback loop additional information, and is likely to not exceed 8k maximum token length. 50/111 Solved

## Overview

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
- https://www.youtube.com/watch?v=plVRxP8hQHY - LLMs as a system of expert agents. Notebooks are the one on 16 Jun 2023, as well as the more updated one on 22 Jul 2023.

These are the experimental results for 111 ARC Training Set problems.

Result:
Solved - 49
Partial Solve (Test Input not correct, but Task Demonstration is correct) - 3
Unsolved - 59

Only 111 were used because we were trying to fit to the 8k context length of GPT4-API and web browser. 
We eventually settled on 3k tokens with object view to cater for the multiple abstraction views.


expert_types = ''
if object_view: 
    expert_types += 'obj'
    if diag: expert_types += 'diag'
    if multicolor: expert_types += 'multi'
    if by_color: expert_types += 'by_color'
    if by_row: expert_types += 'by_row'
    if by_col: expert_types += 'by_col'
    if more_info: expert_types += 'moreinfo'
if pixel_view: expert_types += 'pixel'
if missing_color: expert_types += 'missing_color'

# improving_my_coding_skills
## Dynamic Programming: https://github.com/kothariji/30-days-of-Dynamic-Programming?tab=readme-ov-file
### Snapsack problem:
0/1 recursive snapsack : https://www.youtube.com/watch?v=mGfK-j9gAQA

idea: returning max between if we add each element or we skip it


Fractional Knapsack : https://www.geeksforgeeks.org/fractional-knapsack-problem/

idea: sort array by ratio (profit/weight), and include items from heighest to lowest, fully if possible, otherwise portion until full bag


### balanced parentheses checker with stack:
'''
def is_balanced_parentheses(string):
stack = Stack()
    for char in string:
        if char == '(':
            stack.push(char)
        elif char == ')':
            if stack.is_empty():
                return False
            stack.pop()
    return stack.is_empty()
'''

Explanation of solution: This function iterates through each character in the input string. If an opening parenthesis is encountered, it is pushed onto the stack. For a closing parenthesis, the function checks if the stack is empty (unmatched closing parenthesis) or pops from the stack (matching pair found). At the end, if the stack is empty, all parentheses are balanced; otherwise, they are not.

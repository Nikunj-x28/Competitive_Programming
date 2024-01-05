In questions where simpler sliding windows fail
and the question constraints state that only a limited set of values is part of input (eg only a-z or A-Z) it may be beneficial to

1) Look the answer for each value of input. That is for example first find the result for a , then b , then c and so on...

2) Redefine the task as find windows ending with 'a' that satisfy the particular condition given in the question.

Do this question for practice of the above idea

https://leetcode.com/problems/count-complete-substrings/description/
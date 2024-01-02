Given a permuation [1....n] we want to find an arrangement such that the minimum difference between any two adjancent elements is maximized.

Lets have d be the max min difference
then 1 2 3 4 5 .... d d+1 d+2 ... n 
we can pair 1 d , 2 d+1 , 3 d+2 , ...
Now we want to maxmize this d value but there must be the following condition that this d 
must satisfy :

num + d should exist or num-d should exist in permutation

otherwise
if num +d doesnt exist num + d+1 and higher wont exist same with num-d and lower

so no matter which number we pair our "num" with the minimum difference will be less than d.

visually ->
[num-d][....num....][num+d]  

as the num-d and num+d dont exist in permutaion no matter where we put num the minimum
adjancent difference will be less than d.

Now how to find the right value of d?
See if we can satisfy the num+-d existence for the middle element of permutation

[.....mid.....] 

if mid+d exist or mid-d exist 
then for all numbers one of num+-d will exist
## The highest value of d that satisfies this condition is clearly as we can observe is n/2 .
## As mid+n/2 always exists.

example 
n=9

mid =5 

mid+n/2= 5 +9/2 = 5+4=9

example n=8

mid=4

mid+n/2= 4 + 8/2 = 4+4=8




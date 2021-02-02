Dynammic Programming 

Dynamic Programming is an algorithmic approach to solve some complex problems easily and save time and number of comparisons by storing the results of past computations. The basic idea of dynamic programming is to store the results of previous calculation and reuse it in future instead of recalculating them.

We can also see Dynamic Programming as dividing a particular problem into subproblems and then storing the result of these subproblems to calculate the result of the actual problem.

Consider the problem to find the N-th Fibonacci number.

We know that n-th fibonacci number fib(n) can be defined as:
fib(n) = fib(n-1) + fib(n-2), where n >= 2.

and,

fib(0) = 0 
fib(1) = 1

We can see that the above function fib() to find the nth fibonacci number is divided into two subproblems fib(n-1) and fib(n-2) each one of which will be further divided into subproblems and so on.

The first few Fibonacci numbers are:
1, 1, 2, 3, 5, 8, 13, 21, 34,........

The recursive program to find N-th Fibonacci number is shown belo
int fib(int n) 
{ 
    if (n <= 1) 
        return n; 

    return fib(n-1) + fib(n-2); 
} 

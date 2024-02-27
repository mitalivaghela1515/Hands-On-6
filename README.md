1. Implement both versions of quicksort (random and non-random choice for the pivot) and share the GitHub repository with your source code.

2.  For the non-random pivot version of quicksort show the following benchmarks on the same graph:

    2a) best case (generate a set of inputs that will always be the best case, repeat for multiple array input sizes "n").

    2b) worst case (generate a set of inputs that will always be the worst case, repeat for multiple array input sizes "n").

    2c) average case (generate a set of inputs from a uniform distribution, repeat for multiple array input sizes "n").


    

4. Mathematically derive the average runtime complexity of the non-random pivot version of quicksort.

Ans: -

Let's look at the recurrence relation that characterizes the behavior of the algorithm to determine the average runtime complexity of the non-random pivot version of quicksort.

The array is divided using a selected pivot element in the non-random pivot variant of quicksort. The following represents the recurrence relation for the worst-case temporal complexity:

T(n)=T(n-1) +T(0) +0(n)

In this case, the temporal complexity for an array of size n is represented by T(n). According to the recurrence relation, the time complexity of an array of size n is equal to the product of the time complexities of the subarrays of size n−1 and 0, as well as the O(n) partitioning step.

Let's now calculate the average-case temporal complexity. We assume that the pivot is selected evenly at random in the average situation. Let X X be the random variable that, following partitioning, represents the size of the smaller subarray. The following is an expression for the average-case time complexity:
                                                                    


T(n)=  1/n ∑_(i=0)^(n-1)▒〖(T(i)+T (n-i-1)+O (n)〗


The chance of selecting any element as the pivot is represented as 1/n In this case, and the sum considers all possible pivot positions between 0 and n − 1.

We can solve the recurrence relation using the Master Theorem or other techniques to reduce this statement. Because the subproblems in this situation are not of the same magnitude, the Master Theorem cannot be applied directly; rather, it can be applied to specific words inside the total.

The non-random pivot version of quicksort typically has an average-case time complexity of O (n log n) but depending on the assumptions made about the randomness of pivot selection, the precise mathematical derivation may require probabilistic methods and require a more thorough analysis.




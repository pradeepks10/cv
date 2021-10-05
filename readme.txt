 i have created new file for coding
 Q. Workout time complexities of removing all duplicates in a sorted and unsorted list. Use Binary search and counting sort, if required.

I used to Binary Search  for sorted list and below the their Time complexity of Worst case, Best case and Average case. 
1.Worst case O(log n) 
The O(log n) that we use when talking about Big O has a base of 2. The number of elements is “n” and our time complexity would be the power to which we would raise two to in order to reach n elements. 
2.Best case O(1) 
The best case of binary search is when the first comparison/guess is correct(the key item is equal to the mid of array). It means, regardless of the size of the list/array, we’ll always get the result in constant time. So the best case complexity is O(1).
3.Average case O(log n) 
O(1) means it requires constant time to perform operations like to reach an element in constant time as in case of dictionary and O(n) means, it depends on the value of n to perform operations such as searching an element in an array of n elements. But for O(Log n), it is not that simple. 
At Iteration 1,
Length of array = n
At Iteration 2,
Length of array = n⁄2
At Iteration 3,
Length of array = (n⁄2)⁄2 = n⁄22
Therefore, after Iteration k,
Length of array = n⁄2k
Also, we know that after
After k divisions, the length of array becomes 1
Therefore
Length of array = n⁄2k = 1
	N = 2k
Applying log function on both sides:
=> log2 (n) = log2 (2k)
=> log2 (n) = k log2 (2)
As (loga (a) = 1) 
Therefore,
	K = log2 (n)
Hence, the time complexity of Binary Search is

Log2 (n)
I used to Counting sort algorithm for unsorted list and below the Time complexity of Worst case, Best case and Average case. 
1.Worst case O(n+k) 
I looked at it in this way, there is one run in A[] for getting the maximum element and one more run to store the frequency of each element. This takes O(N) . Therefore, the worst-case time complexity is O(N + K) .
2.Best case O(n+k) 
On the output pass of a counting sort, the array of k counts is read, and array of n elements is written. So there are k writes (to zero the counts), n reads, then k reads and n writes for a total of 2n + 2k operations, but big O ignores the constant 2, so the time complexity is O(n + k).
3.Average case O(n+k) 
The array A is traversed in O(N) time and the resulting sorted array is also computed in O(N) time. Aux[] is traversed in O(K) time. Therefore, the overall time complexity of counting sort algorithm is O(N+K).




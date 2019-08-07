# Interview Tips and Tricks

## Nothing beats practice. Go fucking practice.

Okay for the real advice. I have felt out that most standard 'hard' questions (and of course more challenging ones) involve multiple solutions. Therefore, it is your job to clarify and see what solution space is possible and how to achieve it.

#### Basic steps: ####

1. Brute force / Manually iterate through all possible combinations
2. Use some sort method to get the data in a more organized manner, thus making it easier to compute the solution
3. Use some data structure to get the data in a more organized manner
4. Speaking of data structures, you might have to use algorithms and sorting on top of data structures, such as for DP
5. If they say 'must be in-place' and must have O(1) space complexity, then you have a challenge. You'll have to think of clever ways to reduce the solution to O(n) most likely. You can try using a couple pointers or perhaps some variation on quicksort for O(n) time and O(1) space

#### General Rules of Thumb: ####

* The harder and more competitive a company, the more obscure and less used data structures will be asked for in an 'optimal' solution.
* For example, for a AR startup, I realized I needed to implement Hough Transform instead of using a hash table. I knew of Hough but was not familiar enough to be able to think of it and apply it as a solution.
* Generally the idea is to get brute force down and examine the solution and find bottlenecks. Once found, use anything you can to improve upon the runtime. Rinse and repeat.
* IMHO, Google is the Gold Standard for interviews. Nothing outside the box (like Hough Transform). You'll be expected to give solid performances on all interviews onsite (at least from my experience) in order to pass. Nothing spectacular but needs to be solid from all 4 interviewers. The harder and more coveted companies also throw in design questions and expect you to know their tech stack.

#### General interview question goals: ####

* Get from exponential to polynomial
* Reduce from O(n^3) to O(n^2 * logn) to O(n^2) to O(n * logn) to O(n) and very rarely to log(n) if you're trying to use binary search or something...

#### What data structures to know: ####

* Hashtables
* Graphs
* Heaps
* Stacks
* Queues
* Hashsets
* Tries
* Lists

What sorting methods to know:

* Mergesort
* Radix sort
* Quicksort (great use case: helps find kth element in linear time)

Misc Tips:

* When you end up brute force iterating through the solution space, quite often there is a DP solution that can help reduce runtime. Take time to analyze situation and see where you can reuse computation. One such example is during Google interview where you find number of possible ways to decode an number string. It was originally encoded as A -> 1, B -> 2, etc. 
* When you have to find top k of something, chances are there is an answer that involves heaps. Examples: Find Kth smallest element in sorted matrix. Find the median of an integer stream (for this example, k is half of the input length). Sort and then binary search is another plausible answer for questions that involve finding the k'th element.
* For problems involving finding a duplicate (or finding a "happy number"), can use the linked list cycle detection method of using 2 pointers, one fast and one slow (when slow enters cycle, fast is k steps ahead --> this means if they meet, slow will have moved x steps and fast will have moved k + 2x steps --> thus the formula becomes k + 2x = x --> x = -k --> they meet k steps before entry point)
* Code readability is really important. Simplicity is key.

General flow of interview question should be:
* Solution conception
* Solution explanation via example
* Solution discussion about run and space complexity
* Improve solution if possible, otherwise code the solution

Rehash of above points:
* Discuss solution
* Optimize solution
* Double check solution is applicable to the question at hand
* Try to make simple
* Write clear and readable code


[More advice written a while back](https://medium.com/@Stoic.Sleeper/tips-on-new-grad-software-interviews-27d91fbb31a#.sn8rtwhxa)

# interview-tips-and-tricks

## Nothing beats practice. Go fucking practice.

Okay for the real advice. I have felt out that most standard 'hard' questions (and of course more challenging ones) involve multiple solutions. Therefore, it is your job to clarify and see what solution space is possible and how to achieve it.

#### Basic steps: ####

1. Brute force / Manual iteration through all possible combinations
2. Use some sort method to get the data in a more organized manner, thus making it easier to compute the solution
3. If sorting not valid option, use some data structure to get the data in a more organized manner
4. Speaking of data structures, you might have to use algorithms and sorting on top of data structures, such as for DP
5. If they say 'must be in-place' and must have O(1) space complexity, then you have a problem. You'll have to think of clever ways to reduce the solution to O(n) most likely. You can try using a couple pointers or perhaps

#### General Rules of Thumb: ####

* The harder and more competitive a company, the more obscure and less used data structures will be asked for in an 'optimal' solution.
* For example, for a AR startup, I realized I needed to implement Hough Transform instead of using a hash table. I knew of Hough but was not familiar enough to be able to think of it and apply it as a solution.
* Generally the idea is to get brute force down and examine the solution and find bottlenecks. Once found, use anything you can to improve upon the runtime. Rinse and repeat.
* I say Google is the Gold Standard for interviews. Nothing outside the box (like Hough Transform). You'll be expected to give solid performances on all interviews onsite (at least from my experience) in order to pass. Nothing spectacular but needs to be solid from all 4 interviewers. The harder and more coveted companies also throw in design questions and expect you to know their tech stack.

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
* Quicksort

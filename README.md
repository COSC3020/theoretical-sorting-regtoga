# Theoretical Sorting

A Computer Science researcher claims to have come up with a sorting algorithm
that can sort arbitrary elements in $O(n)$ time based on comparisons of two
elements at a time. This would be asymptotically faster than any known general
sorting algorithm. The algorithm itself is proprietary and will be sold by a
company.

How would you verify this claim? You may assume that you have access to a
black-box implementation of the sorting algorithm, i.e. you cannot examine the
source code, but you can use it to sort any list you like. Explain in detail
your method for investigating whether X is correct, including any expected
results you would get.

Also give a theoretical argument for why X could or could not be correct, based
on the complexity of the general sorting problem we covered in class.

Add your answers to this markdown file.

The way i would initially go about verifying if it is a $O(n)$ runtime is to graph it. If i graphed it a bunch of values untill it started running too slow i would get a pretty good idea of its runtime. I would at the same time graph a known sorting algorithm such as Quicksort ($O(nlogn)$) and insertion sort($O(nlogn)$). I would do Quick sort because it generally runs the fastest and insertion sort because best case it is also $O(n)$. I would make a script that keeps running larger and larger input sizes untill it takes longer than 10 min to run on my machine for each algorithm. This way by the end i can also compare the size of n that each algorithm got to. Once i get my results and make my graph i would look at it and if the mystery algorithm is close to being a straight line i would believe them. i would also want for it to be the fastest algorithm for sorting.

For a theoretical argument as to why X could not be correct, I recall in class you talking about how a sorting algorithm of time complexity $O(n)$ shouldnt be possible becase that doesnt leave for any room to actually compare any number of elements to any other elements. Since there are n! posible orderings of n elements and each comparison partitions the possibilites in two groups, the number of comparisons we would need is atleast $\log_{2}(n!) = \Theta( n\log(n))$

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.
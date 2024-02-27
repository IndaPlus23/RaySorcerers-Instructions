# Quicksort

This is the last assignment of DD1338!

It is obligatory for all students of the course, regardless of being a plus group or not, to have implemented the quicksort algorithm.

Your assignment this week is therefore of course to implement the quicksort algorithm. On top of implementing the fundamental algorithm you also need to optimize it by using insertion sort for smaller arrays and picking a pivot element cleverly, or any other technique. Try to get on the leaderboard!

To pass the assignment you need to have passed the Kattis assignment. (link below)

Info about quicksort and some well-known optimizations can be read about on [Wikipedia](https://en.wikipedia.org/wiki/Quicksort).

## Instructions

1. Create a repository named `<KTH-ID>-quicksort`.
2. Clone your newly created repository and start coding.
3. Submit your solution to [Kattis](https://kth.kattis.com/courses/DD1338/algdat23). (the assignment might not yet exist on Kattis)
4. Upload a screenshot of passing the Kattis tests to your repo here.

## Note on input

The Kattis assignment states that you should make a Java class who's function it's supposed to invoke. You plus students of course want to be able use other languages as well and have granular control over input so you can achieve maximum speed. For this it is still possible to read the input from stdin (input from command line) and output your answer to stdout (output into command line). The format Kattis follows for the assignment is as follows.

It begins with the number of elements to sort followed by every element, separated by spaces:
```
3 2 1 3
```
After sorting these elements you output them sorted on one line seperated by spaces:
```
1 2 3
```

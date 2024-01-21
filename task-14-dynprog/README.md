# DD1338 Week 14
Original Author: Viola Söderlund. 
2024: Edits by Daniel S and Benjamin W.

## Dynamic Programming (mostly)! 
If you haven't tried dynamic programming before, you are in for a treat! This week you are going to experience the pain(pleasure) of optimising a problem to make it go from having a runtime of a few hours, down to under a second.

![](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.redd.it%2Foy8znwiq1b111.png&f=1&nofb=1)

### Prepare for your assigment

1) Create a repository named `<KTH_ID>-dynprog`
2) Clone your newly created repository and start coding. 

To make your Kattis-experience easier, see `./kattis_template/src/main.rs`. If you're mot all förmodan using Java, make use of [this utility class](https://open.Kattis.com/download/Kattio.java?1a0093=) to simplify input-output fast enough to satisfy the judge.

## Assignment
This week, like some other weeks, you may choose between two different assignments:

- Solve LAB2 from _DD2350 Algoritmer, Datastrukturer och Komplexitet_
- (or easier) Solve an ADK exercise problem and some other Kattis problem.

The idea is that you will work with dynamic programming this week no matter which assignment you choose. Of course, you can also do the regular Java assignment.

### ADK LAB2
[Here](https://kth.instructure.com/courses/21037/assignments/124042) you will have access to preparatory questions for the lab. On the same page you will find "[Labblydelsen](https://kth.instructure.com/courses/21037/assignments/124028)", which is where you want to head to find the instructions for the lab itself. Note: you can't access the Java file mentioned in the instructions so you will have to implement the base code yourself.

You will also find the link to the [Kattis problem](https://kth.kattis.com/courses/DD2350/adk23/assignments/owpvwm/problems/kth.adk.spelling) that you need to pass for this assignment. We have provided you with test cases and a big input file to test locally. This is the same input format as Kattis!

>*NOTE*: If testing with the big file, head to the end and after `#`, replace the letters with full words to get better results!

ADK can be quite stressful, but enjoyable! We really recommend solving this, as it is a really fun assignment and it will help you in a few years :). 

#### INDA Adaptation Disclaimer
1) I will accept a solution in any language, not only in Java.
2) I will accept a submission which gives _Time Limit Exceeded_ on Kattis, but passes the provided tests.

#### Solutions
1) Look into _Levenshtein distance_. Construct matrixes of the accumulated costs of the distance between two words. See distance table below:
```
  m a t *
 /-------
m|0 1 1 1
i|1 1 2 2
l|1 2 2 3
e|1 2 3 3
 \-------
```
2) For optimizing: look into search algorithms in weighted graphs, such as _Dijkstra's Algorithm_. Construct a trie of the target words. Search along the trie and use the distance rules as weights.

### ADK exersice + Kattis

If the above ADK problem is too difficult, we have provided you an alternative!

- Solve two in total. 
    - one from `./Assignment.pdf` and
    - one of the followning Kattis problem list regarding graphs and dynamic programming:
      - [Single source shortest path, non-negative weights](https://open.kattis.com/problems/shortestpath1)
      - [All Pairs Shortest Path](https://open.kattis.com/problems/allpairspath)
      - [Proving Equivalences](https://open.kattis.com/problems/equivalences)
      - [Bond](https://open.kattis.com/problems/bond)
      - [Entertainment Box](https://open.kattis.com/problems/entertainmentbox)

The first problem from the PDF is the easiest. There's plenty of Kattis problems to choose from. Feel free to solve muliple of them.

### Grading

For the ADK problem, see _INDA Adaptation Disclaimer_. Always include screenshots of Kattis to prove solution.

If you decide to do any of the non-Kattis exercises from the Multiple Problems category, we require you to write tests to prove the validity of your code.

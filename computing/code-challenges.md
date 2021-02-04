Code Challenges
===============

Online
------

* [Hack The Box](https://www.hackthebox.eu/)
    * Hack The Box is an online platform allowing you to test your penetration testing skills and exchange ideas and methodologies with thousands of people in the security field. Click below to hack our invite challenge, then get started on one of our many live machines or challenges.
* [Project Euler](https://projecteuler.net/) - for raw computer science
* [rosalind](http://rosalind.info/) - for bioinformatics
* [leetcode](https://leetcode.com/)
    * Many languages in browser
    * [Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/)
        * ```[1,2,3,4] -> [1,3,6,10]```
* [HackerRank](https://www.hackerrank.com/)
    * [Add two integers](https://www.hackerrank.com/challenges/solve-me-first/problem)
* [GeekForGeeks](https://www.geeksforgeeks.org/)
    * Tutorials
        * [Bubble Sort](https://www.geeksforgeeks.org/bubble-sort/)
    * Paid for courses
* [The Odin Project](https://www.theodinproject.com/)
    * Your Career in Web Development Starts Here
    * Our full stack curriculum is free and supported by a passionate open source community
    * This is the website we wish we had when we were learning on our own
    * We scour the internet looking for only the best resources to supplement your learning and present them in a logical order
* [codewars.com](https://www.codewars.com/)
    * Achieve mastery through challenge
    * Improve your skills by training with others on real code challenges
* [Advent of Code](https://adventofcode.com/)
    * Many code puzzles


* [interactive-coding-challenges](https://github.com/donnemartin/interactive-coding-challenges)
    * 120+ interactive Python coding interview challenges (algorithms and data structures). Includes Anki flashcards. 
    * The provided Anki flashcard deck uses spaced repetition to help you retain key concepts.
    * Categories    
        * Arrays and Strings - 10
        * Linked Lists - 8
        * Stacks and Queues - 8
        * Graphs and Trees - 21
        * Sorting - 10
        * Recursion and Dynamic Programming - 17
        * Mathematics and Probability - 6
        * Bit Manipulation - 8
        * Online Judges - 16
        * System Design - 8
        * Object Oriented Design - 8

Competitions
------------

* [British Informatics Olympiad](https://www.olympiad.org.uk/)


Other
-----

### Tower of hanoi

* [move-three-disks-in-towers-of-hanoi](https://www.khanacademy.org/computing/computer-science/algorithms/towers-of-hanoi/e/move-three-disks-in-towers-of-hanoi) hands on
* [challenge-solve-hanoi-recursively](https://www.khanacademy.org/computing/computer-science/algorithms/towers-of-hanoi/pc/challenge-solve-hanoi-recursively)

```javascript
var solveHanoi = function(numDisks, fromPeg, toPeg) {
    // base case:  no disks to move
    if (numDisks === 0) {
        return;
    }
    // recursive case:
    var sparePeg = hanoi.getSparePeg(fromPeg, toPeg);
    solveHanoi(numDisks - 1, fromPeg, sparePeg);
    hanoi.moveDisk(fromPeg, toPeg);
    solveHanoi(numDisks - 1, sparePeg, toPeg);
};

solveHanoi(5, "A", "B");
Program.assertEqual(hanoi.isSolved("B"),true);
```
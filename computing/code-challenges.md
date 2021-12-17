Code Challenges
===============

Online
------

* [Hack The Box](https://www.hackthebox.eu/)
    * Hack The Box is an online platform allowing you to test your penetration testing skills and exchange ideas and methodologies with thousands of people in the security field. Click below to hack our invite challenge, then get started on one of our many live machines or challenges.
* [Project Euler](https://projecteuler.net/) - for raw computer science
* [FreeCodeCamp - Coding Interview Prep](https://www.freecodecamp.org/learn/coding-interview-prep/)
    * 1000's of mini problems
* [rosalind](http://rosalind.info/) - for bioinformatics
* [leetcode](https://leetcode.com/)
    * Many languages in browser
    * [Running Sum of 1d Array](https://leetcode.com/problems/running-sum-of-1d-array/)
        * ```[1,2,3,4] -> [1,3,6,10]```
* [HackerRank](https://www.hackerrank.com/)
    * [Add two integers](https://www.hackerrank.com/challenges/solve-me-first/problem)
* [codility.com](https://www.codility.com/)
    * Online service for rating programmers - [[interview]]
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

Are code problems _real_ problems?
https://news.ycombinator.com/item?id=27313883
> LeetCode is an excellent collection of problems you’ll never encounter in real life. If you don’t have a computer science background you might learn some things. Otherwise, it’s just solving silly problems for the sake of solving silly problems.
> It reminds me of when my college required linear algebra for my degree. Learning things that I knew without a shadow of a doubt I would never put to use again. 
They are a good training ground, but should not be the be-all and end-all


FizzBuzz
--------

* [[interview]]
* [[python]]

https://news.ycombinator.com/item?id=27313034
> You know how some people think that fizzbuzz is useless, and how no one ever uses fizzbuzz in real life? if you google it, you'll read things like "I have never needed to write fizzbuzz in production in my entire career!" or words to that effect.
> Of course, fizzbuzz is just checking if you grok some super basic programming concepts like logic, branching, and iteration.
> So what if you want to know if someone knows a little bit _more_ than just the basics? It's the exact same story.
> The ability to be able to work with algorithms and puzzle your way out of a problem is kind of important when you're doing some sorts of programming, especially when you need code that scales well (up OR down).
> If you're really bad at it, you might write pessimal code that even overheats your regular laptop; but fortunately most people aren't quite that bad. ;-) 

* [x86-64+AVX2 assembly language (Linux, cpp+gas)](https://codegolf.stackexchange.com/questions/215216/high-throughput-fizz-buzz/236630#236630)
    * The fastest FizzBuzz implementation
    * Loads of system level programming and kernel features (`write` string is slow) #performance [[performance-profileing]]

Competitions
------------

* [bebras.org](https://www.bebras.org/)
    * Bebras is an international initiative aiming to promote Informatics (Computer Science, or Computing) and computational thinking among school students at all ages.
    * [UK Bebras](https://challenge.bebras.uk/) - Algorithmic Code Challenges for primary and secondary
        * National competition
* [British Informatics Olympiad](https://www.olympiad.org.uk/) - national computing competition for schools and colleges. 
* [International Olympiad in Informatics](https://ioinformatics.org/) - international
    * Lots of publications


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

[//begin]: # "Autogenerated link references for markdown compatibility"
[interview]: interview.md "Interview Questions"
[python]: python.md "python3"
[performance-profileing]: performance-profileing.md "Performance Profiling"
[//end]: # "Autogenerated link references"
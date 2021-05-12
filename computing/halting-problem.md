Halting Problem
===============

```
Alan Turing
Found alluring
Machines whose only fault
Was that they would not halt.
-- Karl David
```

* [How Dr. Seuss would prove the halting problem undecidable](http://ebiquity.umbc.edu/blogger/2008/01/19/how-dr-suess-would-prove-the-halting-problem-undecidable/)
    * ```
        Scooping the Loop Snooper
        an elementary proof of the undecidability of the halting problem

        Geoffrey K. Pullum, University of Edinburgh

        No program can say what another will do.
        Now, I won’t just assert that, I’ll prove it to you:
        I will prove that although you might work til you drop,
        you can’t predict whether a program will stop.

        Imagine we have a procedure called P
        that will snoop in the source code of programs to see
        there aren’t infinite loops that go round and around;
        and P prints the word “Fine!” if no looping is found.

        You feed in your code, and the input it needs,
        and then P takes them both and it studies and reads
        and computes whether things will all end as they should
        (as opposed to going loopy the way that they could).

        Well, the truth is that P cannot possibly be,
        because if you wrote it and gave it to me,
        I could use it to set up a logical bind
        that would shatter your reason and scramble your mind.

        Here’s the trick I would use – and it’s simple to do.
        I’d define a procedure – we’ll name the thing Q –
        that would take any program and call P (of course!)
        to tell if it looped, by reading the source;

        And if so, Q would simply print “Loop!” and then stop;
        but if no, Q would go right back to the top,
        and start off again, looping endlessly back,
        til the universe dies and is frozen and black.

        And this program called Q wouldn’t stay on the shelf;
        I would run it, and (fiendishly) feed it itself.
        What behaviour results when I do this with Q?
        When it reads its own source, just what will it do?

        If P warns of loops, Q will print “Loop!” and quit;
        yet P is supposed to speak truly of it.
        So if Q’s going to quit, then P should say, “Fine!” –
        which will make Q go back to its very first line!

        No matter what P would have done, Q will scoop it:
        Q uses P’s output to make P look stupid.
        If P gets things right then it lies in its tooth;
        and if it speaks falsely, it’s telling the truth!

        I’ve created a paradox, neat as can be –
        and simply by using your putative P.
        When you assumed P you stepped into a snare;
        Your assumptions have led you right into my lair.

        So, how to escape from this logical mess?
        I don’t have to tell you; I’m sure you can guess.
        By reductio, there cannot possibly be
        a procedure that acts like the mythical P.

        You can never discover mechanical means
        for predicting the acts of computing machines.
        It’s something that cannot be done. So we users
        must find our own bugs; our computers are losers! 
        ```
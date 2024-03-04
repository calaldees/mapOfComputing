Interview Questions
===================

*  Philipp Hauer's Blog: [Leveling Up in Job Interviews for Software Engineers](https://phauer.com/2022/leveling-up-job-interviews/) 2022
    * Really good summary
* [Twitter](https://twitter.com/pwang_szn/status/1674719490993688577) [leetcode job offers](https://mem.ai/p/EYuaVqZSCIYiDKcM0w80) 
    * //1: Focus on Fundamentals
        * There are 2000+ problems on Leetcode, but only 10-15 basic data sturcture/algos to use in interviews.
        * topics like: Arrays, Sorting Algorithms, Trees etc
        * So the trick is to do the same 150-200 problems on repeat until you know them in ur sleep.
    * // 2: Get Good at Acting
        * the entire interview process is a charade.
        - act like its the first time seeing the problem (even if you've solved it 5+ times while prepping)
        - purposely make bugs so you can "fix them" to show that you are a good problem solver
    * // 3: Cheat
        * you wanna be broke or cheat?
        * i don't mean cheat in the interviews but use resources in the wild!
        > 1point3acres: chinese forum where entire interview Qs are posted. Use G-Translate or make a chinese friend :)
        > Leetcode Discuss: ppl post direct interview Qs lol.
    * // 4: Get Good at Storytelling
        * 50% of the interview is based on your tech skills but more 50% is on "behavioral" aka how you work w/ other ppl.
        * The trick is to have 4-5 good stories that you can use for any question and you mold the story to fit the interviewer's Q
        * P.S - ✨ I wrote this FREE step-by-step mini-course guide to start coding with A.I
        * (Free for now, but not free forever) Check it out: https://t.co/pmDsYC74tK
    * // 5: Master Negotiating
        * If you're spending 100+ hrs prepping, spend at least 10+ research how much each company pays and invest some time in mastering negotiating.
        * Use sites like Blind + Levels to figure out pay bands and use offers to compete w/ your other offers.
        * 

* [We found the Google Secret Hiring Coding Challenge](https://gurgleapps.com/learn/coding/google-foobar-secret-hiring-coding-challenge-part-1)
    * Kids find and document a random code challenge given by Google profiling.
    * [We found Google's secret coding challenge recruitment platform](https://www.youtube.com/watch?v=JnzHl3RTIFc) YouTube 6min

* [Wasting Time in Tech Interviews](https://www.benjamistan.tech/2022/06/26/wasting-time-in-tech-interviews.html)
    * Most interviews don't actually ask the right questions
    * l33t code questions are no real office work
* [Leetcode Considered Harmful](https://www.fullcontextdevelopment.com/qb/leetcode-considered-harmful)
    * > What is leetcode? If you are not familiar with the term, leetcode is a type of coding task, widely used by the word's largest software companies during live interviews that's exploring a candidate's knowledge of elementary computer science concepts: algorithms, data-structures and complexity analysis. This is in stark contrast with the regular job of most developers, where this knowledge is, at best, marginally relevant.
    * > the real goal of any software product, and in turn every software developer, is to solve human problems. 
* [Grokking the Coding Interview: Patterns for Coding Questions](https://www.educative.io/courses/grokking-the-coding-interview)
    * [educative.io](https://www.educative.io/)
        * Courses for interview preparation
* [The Big Tech Coding Interview Framework - Pt 1. Inspect](https://3dtrends.substack.com/p/the-coding-interview-pt-1-inspect)
    * [google sheet](https://docs.google.com/spreadsheets/d/1gy9cmPwNhZvola7kqnfY3DElk7PYrz2ARpaCODTp8Go/edit#gid=0)
* [My experience as a Gazan girl getting into Silicon Valley companies](https://daliaawad28.medium.com/my-experience-as-a-gazan-girl-getting-into-silicon-valley-companies-488062d769a1) Dalia Awad 2021
* [Ask HN: What is your go to idiot-filter question in interviews?](https://news.ycombinator.com/item?id=33899948)

* [HackerEarth - Technical Interview Questions from big tech companies](https://www.hackerearth.com/practice/interviews/)
* [6 Red Flags I Saw While Doing 60+ Technical Interviews in 30 Days](https://meekg33k.dev/6-red-flags-i-saw-while-doing-60-technical-interviews-in-30-days)
* [How To Solve Amazon's Hanging Cable Interview Question](https://www.youtube.com/watch?v=l_ffdarcJiQ)
    * Two poles 50m high. Connected by a rope 80m long. The rope in the middle is 10m off the ground.


* gov.uk [The STAR method](https://nationalcareers.service.gov.uk/careers-advice/interview-advice/the-star-method)
    * situation - the situation you had to deal with
    * task - the task you were given to do
    * action - the action you took
    * result - what happened as a result of your action and what you learned from the experience
* Looking for autonomy - what did the candidate identify and do off their own back

* [Tech Interview Handbook](https://github.com/yangshun/tech-interview-handbook)
    * 💯 Curated coding interview preparation materials for busy software engineers
    * [techinterviewhandbook.org](https://www.techinterviewhandbook.org/)
        * Prepare the CV
        * Ace the interview
        * Negotiate the offer
        * Prepare for the job
* https://github.com/checkcheckzz/system-design-interview
    * Loads of resources and links to engineering blogs

* [FizzBuzz](https://en.wikipedia.org/wiki/Fizz_buzz#Programming_interviews) [_](https://imranontech.com/2007/01/24/using-fizzbuzz-to-find-developers-who-grok-coding/)
    * > Write a program that prints the numbers from 1 to 100. But for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”. For numbers which are multiples of both three and five print “FizzBuzz”.
    * In under 5min (Pro) - in under 10min (A Grade)
    * [Tom Scott commentary and solution](https://www.youtube.com/watch?v=QPZ0pIK_wsc)
    * Optimise - [High throughput Fizz Buzz](https://codegolf.stackexchange.com/questions/215216/high-throughput-fizz-buzz)
* EnvVar
    * ```python
        def get_env(env_name, is_required=True, default=None, is_bool=False):
            """
            Gets a variable from the environment.
            :param env_name: name of the environment variable
            :param is_required: True if the variable is required, False otherwise
            :param is_bool: True if the variable is a boolean variable
                            (represented by integer values 0 or 1)
            :param default: a default value for the variable
            :return: if the variable is set and not is_bool: the value of the variable
                    if the variable is set and is_bool: False for a value of 0 and True for a value of 1
                    if the variable is not set and not required: the default value
                    if the variable is not set and not required and no default value is specified and is_bool: False
                    if the variable is not set and not required and no default value is specified and not is_bool: None
            :raises Exception: if the variable is required but not set
            """
            pass
    ```

5min story background. Who are you, how did you get here

Clarify any assumptions you made subconsciously. Many questions are under-specified on purpose. E.g. a tree-like diagram could very well be a graph that allows for cycles and a naive recursive solution would not work.

How would you test a random number generator
* Monty carlo? pi - 2d grid

you type `google.com` into a urlbar
You have as much time as you like to describe all the facets of computing that now happens
* [What happens when...](https://github.com/alex/what-happens-when)
    * > This repository is an attempt to answer the age-old interview question "What happens when you type google.com into your browser's address box and press enter?"


As an interviewee 
* Explain your reasoning
* Know different methods for solving a problem
* Ask for clarification, if needed
* Elaborate on answers you don't know

* Behavioural interview questions
    * respond with - Situation, Task, Action and Result
* Situational interview questions
* Education interview questions
    * What do you do to stay up-to-date on your technical certifications and knowledge?
* Technical questions
    * [When and How You Should Denormalize a Relational Database](https://rubygarage.org/blog/database-denormalization-with-examples)
    * In micro-service architecture, what are the ways in which services can be interconnected
    * What is the role of continuous integration systems in the automated-build process?
    * Why would you squash a feature branch before when merging upstream?

https://www.forbes.com/sites/laurencebradford/2016/11/17/15-questions-technical-hiring-managers-love-to-ask-interviewees/?sh=18a17742598e
1. When you don’t know the answer to something, what is the first thing that you do?
2. If you could design your dream job, what would it look like?
3. Can you tell me about a side project you've worked on (outside of school or work) in the past year or so?
    * Possibly not overly convinced about this. people with familys and limited time can still be good engineers
4. How did you first learn to program and what was the first thing you built?
    * Guageing exitement
5. Describe a co-workers style
    * Most candidates can't articulate this
6. Which of your managers gets the best results and most value out of you and why?
7.  If I were to ask your last set of coworkers to describe you, what do you think they'd say?
    *  Consider self reflection
8.  Have you made an account on our website and what do you think can be improved about the process?
    * Only applicable if your company has a public visible website
9.  What’s the one thing we haven’t asked you about that you want to make sure we know?

[](https://www.roberthalf.com/blog/how-to-interview-candidates/7-must-ask-tech-interview-questions)
3. Pretend I’m not a tech person. Can you explain [a relevant technology] in simple terms?
8. What are the benefits and the drawbacks of working in an Agile environment? 
9. How do you think further technology advances will impact your job? 
14. What would you hope to achieve in the first six months after being hired? 
15. How do you manage your work-life balance?
    * Assessing how they cope with burnout

[](https://skillcrush.com/blog/answer-the-toughest-tech-interview-questions/)
2. What’s the best part about your current/last job?
3. What’s the most frustrating part about your current/last job?
4. What are three of your weaknesses?

Mine
* What are the new features in the latest release of _your language here_
* Describe what you contributed to your last team/project
* Can you tell me about a project that failed and articulate why
* You are working on a ticket - you have knowledge about the system and the it is used by users - you think you can add some useful functionality that is not directly specified in the ticket - what do you do?


Code Questions
--------------

https://yangshun.github.io/tech-interview-handbook/best-practice-questions

https://leetcode.com/problems/best-time-to-buy-and-sell-stock/

fizzbuzz -> see [[optimisations]] for fizzbuzz drag racing
fibonachi - optimise? - [Python Program to Print the Fibonacci sequence](https://www.programiz.com/python-programming/examples/fibonacci-sequence)
isPrime - optimise?

```python
from typing import List


def method1(prices):
    return max(
        max(prices[i:]) - price
        for i, price in enumerate(prices)
    )

def method2(prices):
    min_index = prices.index(min(prices))
    max_index = prices.index(max(prices[min_index:]), min_index)
    return prices[max_index] - prices[min_index]

def method3(prices):
    pass
    #todo


def maxProfit(prices: List[int]) -> int:
    """
    https://leetcode.com/problems/best-time-to-buy-and-sell-stock/

    You are given an array prices where prices[i] is the price of a given stock on the ith day.

    You want to maximize your profit by choosing a single day to buy one stock and choosing a different day in the future to sell that stock.

    Return the maximum profit you can achieve from this transaction. If you cannot achieve any profit, return 0.
    
    Example 1:
    >>> maxProfit([7,1,5,3,6,4])
    5

    Explanation: Buy on day 2 (price = 1) and sell on day 5 (price = 6), profit = 6-1 = 5.
    Note that buying on day 2 and selling on day 1 is not allowed because you must buy before you sell.

    Example 2:
    >>> maxProfit([7,6,4,3,1])
    0

    Explanation: In this case, no transactions are done and the max profit = 0.
    """
    return method2(prices)


if __name__ == "__main__":
    print("Running timeit benchmark")
    import timeit, random, sys
    def gen_random_prices(numer_of_random_prices):
        return list(
            random.randint(0, sys.maxsize)
            for i in range(numer_of_random_prices)
        )
    average_time_taken = [
        timeit.timeit(lambda: method(gen_random_prices(2000)), number=3)
        for method in (method1, method2)
    ]
    print(f"{average_time_taken=}")

```


* From [How WhatsApp scaled to 1 billion users with only 50 engineers](https://www.quastor.org/p/how-whatsapp-scaled-to-1-billion)
    * Interview Question
        * Implement a BST Iterator class that represents an iterator over the in-order traversal of a Binary Search Tree.
        * Implement the following methods
            * `BSTIterator` - constructor. The root of the BST will be passed in as a parameter. The pointer should be initialized to a non-existent number small than any number in the BST.
            * `hasNext` - Returns true if there exists a number in the traversal to the right of the pointer, otherwise returns false.
            * `next` - Moves the pointer to the right, then returns the number at the pointer. 



QA Questions
-------------

Some of these might be domain specific.
Some word vomit ... these were the first things that came to my head.
I hope the rational for choosing them and the appropriate answers were hopefully decipherable

1. How would you test a random number generator
2. Do they have enough systems experience to setup CI
3. Discuss Real or virtual devices - why
4. What organisation-structure/process would be need to make BDD a worthwhile investment
    * The business would need to be invested in the auditing of requirements
5. Describe a testing abstraction you have created. Why was it needed.
6. Can you describe the 'definition of done' in your last professional role.
7. What metrics would signify 'the quality of your solution'. Give examples (or fallback to suggestions)
8. Can quality practices be applied universally across multiple projects in an organisation? Can you give examples.
9.  What's more important 'speed of releasing' or 'system reliability' - trick question - this is a business decision
10. Multiple stakeholders within an organisation are putting pressure on the development team to fix outstanding issues. One of the senior stakeholders is becoming increasingly forceful with prioritising issues relating to their area of interest. How do you ensure the correct issues are prioritised.
    * Rank issues by scorning them with a documented business process
11. What new technology in the testing space would you be interested in investigating. Why.


Questions to an interviewer
---------------------------

* [Reverse interview](https://github.com/viraptor/reverse-interview)

* When did you last fire someone and why
    * Do they get rid of the dead wood?
* Am I replacing another role or is this expansion
* Can you give examples of HR/staffing issues you have had and how they were resolved
* How long have each of the team members worked on this project and how have they grown
* Where do you see this department in 1 years time + 3 years time
* Can you give an examples of when there was tension in the team and how this was resolved
* Junoior senior balance
* how evaluate performance
* How are the team encouraged to grow
    * hack time?
    * autonomy
* How do you balance technical vs business goals?

* [I Think I Know Why You Can't Hire Engineers Right Now](https://cushychicken.github.io/why-you-cant-hire-engineers/)
    * Technology -> Cool Stuff to Work On
    * Intellection -> Smart People to Work With
    * Certainty -> Repeatability in Work Environment


Running Interviews
------------------

* [How I build and run behavioral interviews](https://www.benkuhn.net/behavioral/)


[//begin]: # "Autogenerated link references for markdown compatibility"
[optimisations]: optimisations.md "Optimisations"
[//end]: # "Autogenerated link references"
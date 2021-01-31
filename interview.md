Interview Questions
===================

https://github.com/yangshun/tech-interview-handbook

* [FizzBuzz](https://en.wikipedia.org/wiki/Fizz_buzz#Programming_interviews) [_](https://imranontech.com/2007/01/24/using-fizzbuzz-to-find-developers-who-grok-coding/)
    * > Write a program that prints the numbers from 1 to 100. But for multiples of three print “Fizz” instead of the number and for the multiples of five print “Buzz”. For numbers which are multiples of both three and five print “FizzBuzz”.
    * In under 5min (Pro) - in under 10min (A Grade)
    * [Tom Scott commentary and solution](https://www.youtube.com/watch?v=QPZ0pIK_wsc)
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

you type `google.com` into a urlbar
You have as much time as you like to describe all the facets of computing that now happens

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
5. How did you first learn to program and what was the first thing you built?
    * Guageing exitement
6. Describe a co-workers style
    * Most candidates can't articulate this
7. Which of your managers gets the best results and most value out of you and why?
11. If I were to ask your last set of coworkers to describe you, what do you think they'd say?
    *  Consider self reflection
12. Have you made an account on our website and what do you think can be improved about the process?
    * Only applicable if your company has a public visible website
15. What’s the one thing we haven’t asked you about that you want to make sure we know?

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
* Describe what you contributed to your last team/project
* Can you tell me about a project that failed and articulate why

Code Questions
--------------

https://yangshun.github.io/tech-interview-handbook/best-practice-questions

https://leetcode.com/problems/best-time-to-buy-and-sell-stock/

fizzbuzz
fibonachi - optimise?
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
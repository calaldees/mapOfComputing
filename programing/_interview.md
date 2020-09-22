Interview Questions
===================

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

How would you test a random number generator

you type `google.com` into a urlbar
You have as much time as you like to describe all the facets of computing that now happens

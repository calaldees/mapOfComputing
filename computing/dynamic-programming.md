Dynamic Programming
===================

* [Dynamic Programming vs Divide-and-Conquer](https://trekhleb.dev/blog/2018/dynamic-programming-vs-divide-and-conquer/)
    * #Fibonacci, binary search and minimum edit distance [[levenshtein-distance]]

* [Dynamic Programming - Learn to Solve Algorithmic Problems & Coding Challenges](https://www.youtube.com/watch?v=oBt53YbR9Kk) YouTube Course - 5 hours
    * #Fibonacci #memoize (see below)
    * Grid memoize (todo)
    * Tabulation (todo)
    * Recipe (todo)
```javascript
function fib(n) {
    if (n <= 2) {return 1;}
    return fib(n-1) + fib(n-2);
}
//or (my one liner)
const fib = (n, memo={2:1, 1:1}) => memo[n] || (memo[n] = fib(n-1, memo) + fib(n-2, memo))
// Try time complexity of fib(50)

console.assert(fib(6) == 8)
console.assert(fib(7) == 13)
console.assert(fib(8) == 21)
```

[//begin]: # "Autogenerated link references for markdown compatibility"
[levenshtein-distance]: levenshtein-distance.md "Levenshtein distance"
[//end]: # "Autogenerated link references"
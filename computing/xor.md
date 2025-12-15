XOR
===


Can be used at [[interview]]

* https://xania.org/202512/01-xor-eax-eax
  * > encryption part of the code, or some kind of sprite routine
  * `mov eax, 0x0` takes 5 steps
  * `xor eax, eax` sets the eax register to 0
  * Used everywhere in the linux kernel


* [That XOR Trick](https://florian.github.io/xor-trick/)
    * > You are given an array of n - 1 integers which are in the range between 1 and n. All numbers appear exactly once, except one number, which is missing. Find this missing number.
    * > The XOR trick: If we have a sequence of XOR operations a ^ b ^ c ^ ..., then we can remove all pairs of duplicated values without affecting the result.
    * ```
          a ^ b ^ c ^ a ^ b     # Commutativity
        = a ^ a ^ b ^ b ^ c     # Using x ^ x = 0
        = 0 ^ 0 ^ c             # Using x ^ 0 = x (and commutativity)
        = c
      ```
    * In-Place Swapping (without intermediary variable)
    * ```
        x ^= y
        y ^= x
        x ^= y
      ```
    * Finding the Missing Number
    * Finding the Duplicate Number
    * > You are given an array A of n + 1 integers which are in the range between 1 and n. All numbers appear exactly once, except one number, which is duplicated. Find this duplicated number.
    * ```
  
      ```
    * Finding Two Missing/Duplicate Numbers

* [A Neat XOR Trick](https://www.mattkeeter.com/blog/2022-12-10-xor/)
  * > `nznrnfrfntjfmvfwmzdfjlvtqnbhcprsg` Within this string, you want to find the first W-character window in which every character is unique.
  * Give each letter a maskable unique integer bit


[interview]: interview.md "Interview Questions"


regex
=====

Regular Expressions

* [The Regular Expression Visualizer, Simulator & Cross-Compiler Tool](https://blog.robertelder.org/regular-expression-visualizer/)
* [regex101.com](https://regex101.com/)
* [regexcrossword.com](https://regexcrossword.com/)
    * Online web regex game with crosswords - surprisingly fun!
* [rexegg.com](http://rexegg.com)
    * Cookbook
    * [The Greatest Regex Trick Ever](http://rexegg.com/regex-best-trick.html)
        * > How do I match a word unless it's surrounded by quotes?
        * `NotThis|NotThat|GoAway|(WeWantThis)`
* [rulex](https://rulex-rs.github.io/)
    * Enhanced regex that compiles down to regex

* [tweet](https://twitter.com/RegexTip/status/1385604900462137345)
> No regular expression, in the original sense of the term, can match the pattern "any number of a's followed by the same number of b's."
> The slogan is "Regular expressions can't count."

> But here's a "regular expression" in the Perl sense that DOES match any number of a's followed by the same number of b's.
> `(a(?1)?b)`
> The optional (?1) in the middle stands for the outer expression, introducing recursion.


Use find and replace `<.*?>` 
```
<a data-id="extremism" class="glossary" role="link" tabindex="2" aria-label="Extremism. Glossary term.">Extremism</a> is defined as vocal or active opposition to fundamental <a data-id="british-values" class="glossary" role="link" tabindex="2" aria-label="British values. Glossary term.">British values</a>, including <a data-id="democracy" class="glossary" role="link" tabindex="2" aria-label="democracy. Glossary term.">democracy</a>, the <a data-id="rule-of-law" class="glossary" role="link" tabindex="2" aria-label="rule of law. Glossary term.">rule of law</a>, <a data-id="individual-liberty" class="glossary" role="link" tabindex="2" aria-label="individual liberty. Glossary term.">individual liberty</a> and mutual respect and <a data-id="tolerance" class="glossary" role="link" tabindex="2" aria-label="tolerance. Glossary term.">tolerance</a> of different faiths and beliefs.
```

`[^"]+`
Code Quality
============

TODO: port loads of bits over from calaldees/blog?

* [suckless.org software that sucks less: Philosophy](https://suckless.org/philosophy/)
    * > Many (open source) hackers are proud if they achieve large amounts of code, because they believe the more lines of code they've written, the more progress they have made. The more progress they have made, the more skilled they are. This is simply a delusion.

* [Coding on Copilot: 2023 Data Suggests Downward Pressure on Code Quality](https://www.gitclear.com/coding_on_copilot_data_shows_ais_downward_pressure_on_code_quality)
    * > We examine 4 years worth of data, encompassing more than 150m changed lines of code, to determine how AI Assistants influence the quality of code being written. We find a significant uptick in churn code, and a concerning decrease in code reuse. 
    * Graph to show code (churn) rising (quality down)
    * > We find disconcerting trends for maintainability. Code churn -- the percentage of lines that are reverted or updated less than two weeks after being authored -- is projected to double in 2024 compared to its 2021, pre-AI baseline. We further find that the percentage of "added code" and "copy/pasted code" is increasing in proportion to “updated,” “deleted,” and “moved” code. In this regard, code generated during 2023 more resembles an itinerant contributor, prone to violate the DRY-ness of the repos visited. 

* IEEE Software [Developer Productivity for Humans, Part 7: Software Quality](https://ieeexplore.ieee.org/document/10372494)
    * Process Quality
    * Code Quality
    * System Quality
    * Product Quality

* [Boring Python: code quality](https://www.b-list.org/weblog/2022/dec/19/boring-python-code-quality/)
    * This covers most of my points

* Code coverage - CI upwards trend only
* Metrics (cyclomatic complexity)
* Overall metrics
* #pre-commit hooks
    * Formatter
        * Formatter on a legacy codebase

* [refurb](https://github.com/dosisod/refurb) - A tool for refurbishing and modernizing Python codebases 
    * warning about upgrading old python paradigms to use new python3.10+

* [What Makes Code Hard To Read: Visual Patterns of Complexity](https://seeinglogic.com/posts/visual-readability-patterns/)
    * Great article attempting to research a combination of metrics of code readability

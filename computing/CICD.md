Continuous Integration
======================

What is it
Why is it important
Example

Running tests on multiple nodes and combining
Code coverage - reject to lower
pre-commit hooks
code format
Conventional commits
Downstream jobs
Human interaction (authorisation to deploy server or push to app store)
Develop (cooking pot)
Merge restricted (process of approval)
Squash feature commits
    bisect
Artifacts (test reports - audit)
Metrics from Jira
    ticket duration
    feature duration
    story points per sprint
    Cyclomatic complexity
    NOT Lines of Code! (be careful what you measure)
    NOT for the business - a tool for the developers to make judgements


CI + Tests - we dont need to ask permission/approval all the time - we've automated it


* [glci](https://github.com/mdubourg001/glci)
    * Ease GitLab CI Pipelines set-up by running your jobs locally in Docker containers.
* [pre-commit.com/hooks](https://pre-commit.com/hooks.html)
* [GitHub Actions Limitations and Gotchas](https://www.cbui.dev/github-actions-limitations-and-gotchas/)
* 
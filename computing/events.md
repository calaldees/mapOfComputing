Events
======

* [Thinking in Events: From Databases to Distributed Collaboration Software](https://martin.kleppmann.com/2021/07/02/debs-keynote-thinking-in-events.html)
    * Martin Kleppmann

* [Don't let Event-Driven Architecture buzzwords fool you](https://event-driven.io/en/dont_let_event_driven_architecture_buzzwords_fool_you/)
    * > Events are excellent workflow facilitators. They represent facts on what has happened. We’re inverting the classical flow; instead of requesting everything, we’re notifying all interested parties. Then others can react and publish new information through events. That helps to build decoupled and autonomous components.
    * > Events are messages, but they’re not the only message type. The second most important is command. They differ by intention. I wrote about it longer in What’s the difference between a command and an event?. TLDR:
    * A command is an intent to do something. It’s directed, and the handler may reject it.
    * Events are facts; they can (and should) have multiple receivers. Yet, the event producers shouldn’t assume getting a response.
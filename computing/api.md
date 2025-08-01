API
===

TODO: What is an API

http://editor.swagger.io/

* [Advice for Operating a Public-Facing API](https://jcs.org/2023/07/12/api)
    * Avoid OAuth if you can
        * It just makes things gubby - short api tokens are good
    * Log a unique id with every request
    * Be descriptive in your error responses
    * Use prefixed tokens
    * Stay on top of failures
        * When an IP block can be mapped back to a user by way of an API token in the request, that user is sent an automated e-mail explaining why they were blocked and that they need to shut down whatever is continuing to send the failed requests.
        * My solution for this in Pushover's API was to add a step in between the soft and hard block. When a failure count is nearing the hard block limit, Pushover's API will respond with a 200 status code, but with a descriptive message in the body explaining that the message was ignored but the API is responding that way to avoid a catastrophe.

* [API Mandate](https://chrislaing.net/blog/the-memo/) - Jeff Bezos - Amazon 2002
    1. All teams will henceforth expose their data and functionality through service interfaces.
    2. Teams must communicate with each other through these interfaces.
    3. There will be no other form of interprocess communication allowed: no direct linking, no direct reads of another team’s data store, no shared-memory model, no back-doors whatsoever. The only communication allowed is via service interface calls over the network.
    4. It doesn’t matter what technology they use. HTTP, Corba, Pubsub, custom protocols — doesn’t matter.
    5. All service interfaces, without exception, must be designed from the ground up to be externalizable. That is to say, the team must plan and design to be able to expose the interface to developers in the outside world. No exceptions.
    6. Anyone who doesn’t do this will be fired.
    7. Thank you; have a nice day!



Generate server stubs form yaml for range of languages

https://github.com/OAI/OpenAPI-Specification
[[openapi]]

* [JSONPlaceholder](https://jsonplaceholder.typicode.com/) example
    * [guide](https://jsonplaceholder.typicode.com/guide/) in plainjs. can be run in browser debug window
* [yes/no api](https://yesno.wtf/#api)

https://github.com/kotartemiy/newscatcher/blob/master/README.md

* [API Improvement Proposals](https://google.aip.dev/)
    * Focused design documents for flexible API development

* [openvisionapi.com](https://openvisionapi.com/)
    * API for object identification from images

* [Micro APIs - Programmable building blocks for everyday use](https://blog.m3o.com/2021/06/24/micro-apis-for-everyday-use.html)
    * commercial project of useful services

[[authentication]]

REST Apis are a human abstraction
[[mcp]] is an abstraction for [[llm]]s

[//begin]: # "Autogenerated link references for markdown compatibility"
[openapi]: openapi.md "OpenAPI"
[authentication]: authentication.md "Authentication"
[mcp]: mcp.md "MCP (Model Context Protocol)"
[llm]: llm.md "Large Language Models"
[//end]: # "Autogenerated link references"
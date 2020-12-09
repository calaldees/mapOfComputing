UI - User Interfaces
====================

* tweet [Blackboard is aweful, here is why](https://twitter.com/dreen_gb/status/1335898204936806400) Greg Balaga @dreen_gb

[Windows 95](https://twitter.com/tuomassalo/status/978717292023500805)
Discoverability
    * See 98.css [css](./css.md)

[Web Desktops](https://simone.computer/#/webdesktops)
windows 93
EmuOS

[The Distribution of Users’ Computer Skills: Worse Than You Think](https://www.nngroup.com/articles/computer-skill-levels/)

[hacker news discussion](https://news.ycombinator.com/item?id=21037674)

https://threadreaderapp.com/thread/927593460642615296.html
> one of the primary reasons computers were *created* was to cross reference data. that is nearly impossible in most software now.
> You don't even realize why the process is frustrating because it's just The Way It Is.
> Mice are great for unstructured data - wikipedia - twitter,google dopbox are linear

* [The Decline of Usability](https://datagubbe.se/decusab/)
* [The Humane Interface](https://en.wikipedia.org/wiki/The_Humane_Interface) - 2000 Jef Raskin
    * The book puts forward a large number of interface design suggestions, from fairly trivial ones to radical ones. The overriding theme is that current computer interfaces are often poor and set up users to fail, as a result of poor planning (or lack of planning) by programmers and a lack of understanding of how people actually use software. 
        * Modelessness - dispose of the caps-lock key - (sustained physical action)
        * Every action should be undoable, even after a document or application has been closed and reopened.
        * warning screen ... are unhelpful because users tend to ignore them out of habit,
        * graphic icons in software without any accompanying text are often cryptic to users
        * there should be only one way to accomplish a certain atomic task 

Bluring the lines
Ad's and content indistinguishable?
(link to psycology.md?)
https://twitter.com/craigmod/status/1219644556003565568

Perceived performance

Carousels are a terrible pattern
    nobody knows how to use them
    The're reading and it moves
    They are are just to resolve busines fights about what's at the top
    this solves Business problem not the users problem

Be predictable - keep to conventions - comfortable

Accessibility is not optional

Play at speed
ADOM


[Windows Explorer Through The Years](https://gekk.info/articles/explorer.html)

Graphic Design
--------------

https://uxdesign.cc/7-principles-of-icon-design-e7187539e4a2
TODO: look at uxdesign site further ...

UX
--

https://blurha.sh/


Game Interfaces
---------------

http://www.atlasoftheuniverse.com/12lys.html
Tie-Fighter - radar

CLI
---
common paradimes
flags, positional params, named params, pipes?
[Command Line Interface Guidelines](https://clig.dev/)
[commandLine.md](./commandLine.md)

investigate!
https://github.com/ivanreese/visual-programming-codex


libs

https://tailwindui.com/


Voice
-----

### [rhasspy](https://github.com/rhasspy/rhasspy#rhasspy-voice-assistant)
* [docs](https://rhasspy.readthedocs.io/)
* [Overview of Rhasspy 2.5](https://www.youtube.com/watch?v=IsAlz76PXJQ)

```bash
    docker run \
        -p 12101:12101 \
        --name rhasspy \
        --restart unless-stopped \
        -v "$HOME/.config/rhasspy/profiles:/profiles" \
        -v "/etc/localtime:/etc/localtime:ro" \
        --device /dev/snd:/dev/snd \
        rhasspy/rhasspy \
        --user-profiles /profiles \
        --profile en
```

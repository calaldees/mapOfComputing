UI - User Interfaces
====================

* [Collection of Human Interface and Software Design Guides](http://www.geofcrowl.com/blog/articles/2020/2/17/collection-higs/)

* Android
    * [Material Design](https://material.io/)
        * [Material Icons](https://fonts.google.com/icons) searchable

* tweet [Blackboard is aweful, here is why](https://twitter.com/dreen_gb/status/1335898204936806400) Greg Balaga @dreen_gb

[Windows 95](https://twitter.com/tuomassalo/status/978717292023500805)
Discoverability
    * See 98.css [css](./css.md)
* Interact with windows95 ui in browser from [[web-operating-systems]]


* [The Universe of Discourse - Fuckin' user interface design, I swear](https://blog.plover.com/tech/ui.html)
    * Don't have your destructive operations near the common path operations
* [Why We Need to Rethink the Computer ‘Desktop’ as a Concept](https://onezero.medium.com/the-document-metaphor-desktop-gui-doesnt-work-anymore-d276271bfa40) - Thoughts about a new direction for desktop UI
    * Keep every user interacted fragment, store metadata, make it searchable, across all applications (cloud or otherwise)

[The Distribution of Users’ Computer Skills: Worse Than You Think](https://www.nngroup.com/articles/computer-skill-levels/)

[hacker news discussion](https://news.ycombinator.com/item?id=21037674)

https://threadreaderapp.com/thread/927593460642615296.html
> one of the primary reasons computers were *created* was to cross reference data. that is nearly impossible in most software now.
> You don't even realize why the process is frustrating because it's just The Way It Is.
> Mice are great for unstructured data - wikipedia - twitter,google dopbox are linear

* [The Rise Of User-Hostile Software](https://den.dev/blog/user-hostile-software/) Or why software we get today is not the software we should strive to be getting tomorrow.
* [The Decline of Usability](https://datagubbe.se/decusab/)
* [The Humane Interface](https://en.wikipedia.org/wiki/The_Humane_Interface) - 2000 Jef Raskin
    * The book puts forward a large number of interface design suggestions, from fairly trivial ones to radical ones. The overriding theme is that current computer interfaces are often poor and set up users to fail, as a result of poor planning (or lack of planning) by programmers and a lack of understanding of how people actually use software. 
        * Modelessness - dispose of the caps-lock key - (sustained physical action)
        * Every action should be undoable, even after a document or application has been closed and reopened.
        * warning screen ... are unhelpful because users tend to ignore them out of habit,
        * graphic icons in software without any accompanying text are often cryptic to users
        * there should be only one way to accomplish a certain atomic task
* [Remembering Windows 3.1 themes and user empowerment](https://hisham.hm/2019/07/26/remembering-windows-31-themes-and-user-empowerment/)
    * You used to have ownership and customisation of your machine
* [Habits, UI changes, and OS stagnation](https://morrick.me/archives/9407)
    * Apple redesigned the look of their UI each year is just annoying to users. Shuffle things around is not progress


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

* [NYXT Browser: visual-mode: mouse-free copy](https://nyxt.atlas.engineer/article/visual-mode.org)
* [User power, not power users: htop and its design philosophy](https://hisham.hm/2020/12/18/huser-power-not-power-users-htop-and-its-design-philosophy/)

[Windows Explorer Through The Years](https://gekk.info/articles/explorer.html)

Graphic Design
--------------

https://uxdesign.cc/7-principles-of-icon-design-e7187539e4a2
TODO: look at uxdesign site further ...

* [[color]] theory

Tween/Ease functions [[css]]

UX 
---

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

[//begin]: # "Autogenerated link references for markdown compatibility"
[web-operating-systems]: web-operating-systems.md "web-operating-systems"
[color]: color.md "Color"
[css]: css.md "CSS"
[//end]: # "Autogenerated link references"
Terminal
========

* See also [[cli]]

* [the-art-of-command-line](https://github.com/jlevy/the-art-of-command-line) in one page
  * bash trial

* [[bash]]

* [Terminal colours are tricky](https://jvns.ca/blog/2024/10/01/terminal-colours/)
  * Getting colors correct in terminals is tricky
* [Terminals should generate the 256-color palette ](https://gist.github.com/jake-stewart/0a8ea46159a7da2c808e5be2177e1783)
  * Terminals normally only use 16 colors or TrueColor (wow), but if we could have something in-between? great writeup of use cases and compatibility
* [ANSI Escape Codes](https://ansi.tools/) previewed in browser
  * cursor up, cursor down

Terminal
--------

Do not use the default terminal on any system. This will hinder your productivity.

* https://www.jeffquast.com/post/state-of-terminal-emulation-2025/
  * https://ucs-detect.readthedocs.io/results.html
    * Ranking terminal emulators for accuracy

* Multiplatform
  * [Contour Terminal Emulator](http://contour-terminal.org/)
    * high dpi - win, linux, mac
  * [Alacritty](https://github.com/alacritty/alacritty) multi-platform terminal
  * [WezTerm](https://wezfurlong.org/wezterm/) - is a GPU-accelerated cross-platform terminal emulator and multiplexer written by @wez and implemented in Rust
  * Electron
    * [Hyper](https://hyper.is/)
    * [Terminus](https://www.electronjs.org/apps/terminus)
  * Fun
    * [edex-ui](https://github.com/GitSquared/edex-ui)
* OSX
  * [iTerm2](https://www.iterm2.com/)

automation - dont copy and paste manually.
  - get me a list of all the files in the structure
  - now compress them and put them on a webserver

Shells
------

* Windows
  * cmd
  * powershell
    * [PSKoans](https://github.com/vexx32/PSKoans) -  A simple, fun, and interactive way to learn the PowerShell language through Pester [[automated-testing]]
  * wsl (bash)
* Linux
  * [Alternative-Shells](https://github.com/oilshell/oil/wiki/Alternative-Shells)
  * sh
  * [[bash]] (5+)
    * (see the bash page for loads of cool tricks/examples for productive developers)
  * zsh


Startup Environment
-------------------

* ~/.bashrc
* ~/.bash_profile
* autoexec?

tab completion


Video
-----

* [Create Vintage Videos Using FFmpeg in 4 Simple Steps](https://ottverse.com/create-vintage-videos-using-ffmpeg/)
* related
  * [Edit videos live with pyhthon](https://github.com/Zulko/moviepy) - automation [[python]]

Desktop Environment
-------------------

* [CONSOLE DESKTOP GUIDE](https://pspodcasting.net/dan/blog/2018/console_desktop.html)
  * Use a terminal for your entire computer
  * tmux (multi window)
  * `lynx` for text based browser
  * Word processors, graphs, progress bars


Performance
----------

* ["Terminal Velocity", a graphics demo running in the Linux Terminal](https://www.youtube.com/watch?v=MWcuI2SXA-A) YouTube 3min
  * If you think that Linux terminals are limited to displaying text, think again!
  * It's quite possible to display graphics with a decent framerate in your terminal. It even works (without sound) over SSH...


[cli]: cli.md "CLI Command Line Interface"
[bash]: bash.md "bash"
[automated-testing]: automated-testing.md "Automated Testing"
[python]: python.md "python3"


Flags
=====

The flags pattern
boolean set of options

Equivilent concept: Tick box's in gui's become `--flag` in commandline

common pattern ...
flags can be integers corresponding to bit flags. This enabled composition by using the `+` operator

https://docs.python.org/3/library/re.html#flags
ASCII and UNICODE flags can be used at the same time, but it does not make sense. There are not multiple fields to complicate the schema
chrome://flags/
https://docs.python.org/3/library/argparse.html#name-or-flags
https://zdoom.org/wiki/DMFlags
https://ffmpeg.org/ffmpeg.html
https://curl.se/docs/manpage.html
https://gobyexample.com/command-line-flags
The pattern of commandline flags
Integer bit flags (cane be combined with `+` because they are integers)
Some of the flags when combined don't make sense,
https://linux.die.net/man/1/rsync 'unexpected results' when some flags are used together
There are also cases where some flags only makes sense when another flag is set ( see chrome://flags/​ #tabstrip-combo-button​ 'Might require tab search toolbar flag to be disabled to take effect')


You are indeed correct that some flags may conflict and be mutually exclusive. This can happen. For example, most regex librarys has a concept of flags. https://docs.python.org/3/library/re.html#flags in python you can have ASCII and UNICODE flags active at the same time, but it's not really valid use. The library designers could have created an additional param called encoding​ (possibly), but they opted for flags probably because of the composeability and may have been trying to reduce the complexity of the setup params. The same pattern appears in other contexts where flags are used, e.g (https://linux.die.net/man/1/rsync has 'unexpected results' when some flags are used together). There are also cases where some flags only makes sense when another flag is set ( see chrome://flags/​ #tabstrip-combo-button​ 'Might require tab search toolbar flag to be disabled to take effect')
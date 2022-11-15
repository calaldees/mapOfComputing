Translation Layer
-----------------


* [Darwin (OSX) on Linux](https://www.darlinghq.org/)
* [Android in a box](https://anbox.io/) - Linux stack for native android

WINE

* [Twister OS](https://twisteros.com/)
    * > vanishes the borders between ARM Linux and x86 Linux, being able to automatically execute (with some kind of success) x86 Linux binaries and Wine x86 without any complex process like we suffer on other slow and painful implementations
* [Hangover](https://github.com/AndreRH/hangover) - runs simple Win64/Win32 applications on arm64/ppc64le/x86_64 Linux and x86_64 Mac

* [The Apple M1, ARM/x86 Linux Virtualization, and BOINC](https://www.sevarg.net/2021/01/09/arm-mac-mini-and-boinc/)
    * The issue is that on x86, if you write memory addresses in a certain sequence, all other cores will see the writes in the same sequence. If you write some blob of data and then write the “Ready!” flag, by the time other cores see the flag change value, you can be certain that the blob of data has been written. ARM has no such guarantees without explicit (and slow) memory barrier instructions, and this is why the x86 emulation on ARM Windows was painful - guaranteeing correctness of a translated binary on a weaker memory model is slow.
    * As it turns out, Apple isn’t doing it purely in software - they have Total Store Ordering support in their hardware! When the M1 runs a translated x86 binary, the OS just tells the chip, “Hey, use x86 memory ordering for this thread.” Things built natively for ARM can take advantage of the performance gains of the memory reordering, and things that requires strict ordering get strict ordering. It’s a very, very clever way to totally bypass the memory ordering issues with translated binaries, and it’s not a thing in any other ARM chip on the planet (I’d say yet, but I really don’t think this will become a popular thing to implement - perks of Apple building their own silicon)

* [Running Intel Binaries in Linux VMs with Rosetta](https://developer.apple.com/documentation/virtualization/running_intel_binaries_in_linux_vms_with_rosetta) - Run x86_64 Linux binaries under ARM Linux on Apple silicon.

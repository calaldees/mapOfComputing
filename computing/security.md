Hacking and Security
====================

* [[2fa]]

* [9Sec Blog](https://9esec.io/blog) - Experts insights
* [Cyber Roadmap by Tux](https://blog.ashimi.xyz/cyber-security-beginner-roadmap-ckk1cmmvb08jfqps1amjuh10o)
    * [tryhackme.com](https://tryhackme.com/) - Byte-sized gamified lessons
    * [immersivelabs.online](https://immersivelabs.online/) - info
    * [hackthebox.eu](https://www.hackthebox.eu/)
        * is very much hard than the previous two because you can't sign up directly, you have to hack your way into the platform. 
    * VulnHub
    * [PEH by TCM](https://academy.tcm-sec.com/p/practical-ethical-hacking-the-complete-course)
        * is a 25 hours course by TCM Security, 
    * Certification
        * [eJPT](https://elearnsecurity.com/product/ejpt-certification/)
        * [Offensive Security Certified Professional (OSCP)](https://www.offensive-security.com/pwk-oscp/OSCP/)
            *  is an ethical hacking certification offered by Offensive Security that teaches penetration testing methodologies and the use of the tools included with the Kali Linux distribution (successor of BackTrack). The OSCP is a hands-on penetration testing certification, requiring holders to successfully attack and penetrate various live machines in a safe lab environment.
        * [Certified Ethical Hacker (CEH)](https://www.eccouncil.org/programs/certified-ethical-hacker-ceh/) certificate of the ultimate pen tester

* 75% of all attacks are phishing
* Social engineering
* Malware
    * virus
    * trogan
* Randomware
* Spyware/adware
* Hacking #DDoS

* fake phishing emails - get data on links/replys - levels of difficulty
* Vishing (voice call phishing)
    * never take unsolicited calls
* multi factor authentication
* passowrd managers (dont use the same password)
    * [](https://howsecureismypassword.net/)

* [pam-duress](https://github.com/nuvious/pam-duress)
    * > A Pluggable Authentication Module (PAM) which allows the establishment of alternate passwords that can be used to perform actions to clear sensitive data, notify IT/Security staff, close off sensitive network connections, etc if a user is coerced into giving a threat actor a password

* [How to share a secret](https://web.mit.edu/6.857/OldStuff/Fall03/ref/Shamir-HowToShareASecret.pdf) pdf paper 2 pages

* [Pure](https://github.com/ronomon/pure) - A static analysis file format checker
    * Check contents of zip files for common invalid file attacks

Active twitter security dude that retweets cool stuff 2023
https://twitter.com/xpldotjs

* [The Most Dangerous Codec in the World: Finding and Exploiting Vulnerabilities in H.264 Decoders](https://wrv.github.io/h26forge.pdf) Willy R. Vasquez, The University of Texas at Austin, Stephen Checkoway, Oberlin College, Hovav Shacham, The University of Texas at Austin
    * > Modern video encoding standards such as H.264 are a marvel of hidden complexity. But with hidden complexity comes hidden security risk. Decoding video in practice means interacting with dedicated hardware accelerators and the proprietary, privileged software components used to drive them. 
    * > The video decoder ecosystem is obscure, opaque, diverse, highly privileged, largely untested, and highly exposed—a dangerous combination.
    * > We introduce and evaluate H26FORGE, domain-specific infrastructure for analyzing, generating, and manipulating syntactically correct but semantically spec-non-compliant video files. Using H26FORGE, we uncover insecurity in depth across the video decoder ecosystem, including kernel memory corruption bugs in iOS, memory corruption bugs in Firefox and VLC for Windows, and video accelerator and application processor kernel memory bugs in multiple Android devices.

You can't add it later

Question: how will you know you've had a data breach?

Users are evil and dumb
Could be hijacked
People are horrible


RSA: Public Private keys

SSH

2 Factor

* [Kontra OWASP Top 10 for API](https://application.security/free/owasp-top-10-API) - Application Security Training
* [Can We Stop Pretending SMS Is Secure Now?](https://krebsonsecurity.com/2021/03/can-we-stop-pretending-sms-is-secure-now/) 2021 Krebs On Security
    * [Phone numbers must die](https://www.devever.net/~hl/e164) - they organisation of the number and reuse is a mess
* [SeaGlass](https://seaglass.cs.washington.edu/) - Enabling City-Wide IMSI-Catcher Detection
    * Identifying rouge celltowers for evesdropping

* [SolarWinds: Why the Sunburst hack is so serious](https://www.bbc.co.uk/news/technology-55321643)
    * Targeted government devices by cyber military team. Payload in software update.
    * [Why the World Needs a Software Bill Of Materials Now](https://drrispens.medium.com/why-the-world-needs-a-software-bill-of-materials-now-5a565df65dff)
        * > The first details on the “Sunburst” attack were released in December 2020: a highly evasive attacker leveraged the supply chain of the U.S. based software company SolarWinds in order to compromise an administrative I.T. management tool which is used by tens of thousands of private and government organizations. The backdoors and malware that were installed on the victims’ infrastructures have been called by Microsoft “the most sophisticated and protracted intrusion attacks of the decade”.
        * > The attack on SolarWinds has made it more apparent than ever before that software supply chain attacks are incredibly destructive. Damage done in a tiny module delivered by a small software vendor can break a global software empire’s security.

U2F

Authenticator app OTP


* [Keytap2 - acoustic keyboard eavesdropping based on language n-gram frequencies](https://github.com/ggerganov/kbd-audio/discussions/31)
    * Audio recording of someone using a computer keyboard in an attempt to decipher from audio alone what keys have been pressed
* [AIR-FI: Generating Covert Wi-Fi Signals from Air-Gapped Computers](https://arxiv.org/abs/2012.06884)
* [Timing Analysis of Keystrokes and Timing Attacks on SSH](https://people.eecs.berkeley.edu/~daw/papers/ssh-use01.pdf)
    * > in inter-active mode,every individual keystroke that a user types is sent to the remote machine in a separate IP packet immediately after the key is pressed, which leaks the inter-keystroke timing information of users’ typing.
* Acoustic Cryptanalysis - Audio SSH RSA key retrieval
    * [New attack steals e-mail decryption keys by capturing computer sounds](https://arstechnica.com/information-technology/2013/12/new-attack-steals-e-mail-decryption-keys-by-capturing-computer-sounds/)
    * [Acoustic Cryptanalysis](https://link.springer.com/article/10.1007/s00145-015-9224-2) 2016
        * [another pdf](https://www.cs.tau.ac.il/~tromer/papers/acoustic-20131218.pdf)
        * > Many computers emit a high-pitched noise during operation, due to vibration in some of their electronic components. These acoustic emanations are more than a nuisance: They can convey information about the software running on the computer and, in particular, leak sensitive information about security-related computations.
        * > The attack can extract full 4096-bit RSA decryption keys from laptop computers (of various models), within an hour, using the sound generated by the computer during the decryption ... using a plain mobile phone placed next to the computer, or a more sensitive microphone placed 10 meters away.
* [How to date a audio recording using background electrical noise](https://robertheaton.com/enf/)
    * Video recordings pic up the audio 'hum' of the national grid. We have accurate data from the national grid, so can pinpoint the time of a recording and tell if it was one doctored clip.
* [Video-based Cryptanalysis BH USA 23 & DEFCON 31 - Exploiting a Video Camera's Rolling Shutter to Recover Secret Keys from Devices Using Video Footage of Their Power LED](https://www.nassiben.com/video-based-crypta)
* Speculative execution (timing vulnerability)
    * [Spectre](https://en.wikipedia.org/wiki/Spectre_(security_vulnerability))
* [Downfall](https://downfall.page/)
    * > The vulnerability is caused by memory optimization features in Intel processors that unintentionally reveal internal hardware registers to software.
    * Stealing 128-bit and 256-bit AES keys from another user (linux Kernel)
    * Computing devices based on Intel Core processors from the 6th Skylake to (including) the 11th Tiger Lake generation are affected
* [spookjs](https://www.spookjs.com/)
    * Vulnerability that gives access to Google Password manager from javascript


* [Technology, as seen on TV](https://fasterthanli.me/series/tech-as-seen-on-tv)
    * TV depictions of technology, and reviewing how realistic they are

* [Hidden OAuth attack vectors](https://portswigger.net/research/hidden-oauth-attack-vectors) Michael Stepankin

Unauthenticaed SMTP

Screenshot of background and relay password (why ctrl+alt+del to login)

Message board with alert('hacked')

School Technitions and network admins about supporting students with security interests

Keyloggers


* [Python 3.10.7 - DDos Fix - CVE-2020-10735](https://pythoninsider.blogspot.com/2022/09/python-releases-3107-3914-3814-and-3714.html) #python #ddos #hex
    * > Converting between int and str in bases other than 2 (binary), 4, 8 (octal), 16 (hexadecimal), or 32 such as base 10 (decimal) now raises a ValueError if the number of digits in string form is above a limit to avoid potential denial of service attacks due to the algorithmic complexity.



Global Radio Login Gigya - 'Hacked by' alert

* [How To Become A Hacker](https://zalberico.com/essay/2020/04/19/how-to-become-a-hacker.html)

* [Dashboard: Zero-Days in Desktop Web Browsers](https://www.radsix.com/dashboard1/)

* [System Bus Radio](https://github.com/fulldecent/system-bus-radio) - transmit radio from air-gapped computers with no radio hardware

* [Stealing Your Private YouTube Videos, One Frame at a Time](https://bugs.xdavidhu.me/google/2021/01/11/stealing-your-private-videos-one-frame-at-a-time/)


* [Project Zero](https://googleprojectzero.blogspot.com/) - News and updates from the Project Zero team at Google
    * [The State of State Machines ](https://googleprojectzero.blogspot.com/2021/01/the-state-of-state-machines.html)
        * Video call mechanisms have state machine logic bugs. Investigating a range of protocols revealed most have state logic bugs
        * Group FaceTime which allowed an attacker to call a target and force the call to connect without user interaction from the target, allowing the attacker to listen to the target’s surroundings without their knowledge or consent. 
* [HeartBleed](https://heartbleed.com/)
* [log4j](https://www.lunasec.io/docs/blog/log4j-zero-day/)
    * Remote code execution on JVM though in logging package
    * [Log4Shell Update: Second log4j Vulnerability Published](https://www.lunasec.io/docs/blog/log4j-zero-day-update-on-cve-2021-45046/)

* [Open Web Application Security Project® (OWASP)](https://owasp.org/) is a nonprofit foundation that works to improve the security of software.
    * [OWASP Cheat Sheets](https://cheatsheetseries.owasp.org/index.html) - how to write security centred software

* [Execute remote code on `git clone`](https://www.openwall.com/lists/oss-security/2021/03/09/3)
    * > CVE-2021-21300: On case-insensitive filesystems, with support for symbolic links, if Git is configured globally to apply delay-capable clean/smudge filters (such as Git LFS), Git could be fooled into running remote code during a clone.
* [This man thought opening a TXT file is fine, he thought wrong. macOS CVE-2019-8761](https://www.paulosyibelo.com/2021/04/this-man-thought-opening-txt-file-is.html)
    * Mac textedit tricked into opening rtf-html from txt file and making a web request, not sandboxed by a web browser proxy settings and leaking the users real ip address
* [Privacy Implications of Accelerometer Data:  A Review of Possible Inferences](https://dl.acm.org/doi/pdf/10.1145/3309074.3309076)
    * we found  that  accelerometer  data  alone  may  be  sufficient  to  obtain information  about  a  device  holder’s  location,  activities,  health condition,   body   features,   gender,   age,   personality   traits,   and emotional state. Acceleration signals can even be used to uniquely identify  a  person  based  on  biometric  movement  patterns  and  to reconstruct  sequences  of  text  entered  into  a  device,  including passwords.
    * [[privacy]]

* [fragattacks.com](https://www.fragattacks.com/) - fragmentation and aggregation attacks
    * a collection of new security vulnerabilities that affect Wi-Fi devices

* [Router Security Vulnerabilities](https://modemly.com/m1/pulse)
    * 8000+

* [Dev corrupts NPM libs 'colors' and 'faker' breaking thousands of apps](https://www.bleepingcomputer.com/news/security/dev-corrupts-npm-libs-colors-and-faker-breaking-thousands-of-apps/)

* [But You Told Me You Were Safe: Attacking the Mozilla Firefox Renderer (Part 1)](https://www.zerodayinitiative.com/blog/2022/8/17/but-you-told-me-you-were-safe-attacking-the-mozilla-firefox-renderer-part-1)
    * From javascript, corrupting the array.prototype to get the module object and binary access to the deterministic JIT compiler to then exploit kernel32.dll on windows. This is MAD!

Fuzzing #fuzzing
-------

* [Fuzzing Modern UDP Game Protocols With Snapshot-based Fuzzers](http://blog.ret2.io/2021/07/21/wtf-snapshot-fuzzing/)
    * #reverse-engineering #fuzzing


Case Studies
------------

Cautionary tails of actual hacks

* [Hackers Break Into Thousands of Security Cameras, Exposing Tesla, Jails, Hospitals](https://www.bnnbloomberg.ca/hackers-break-into-thousands-of-security-cameras-exposing-tesla-jails-hospitals-1.1574681)
* [What Is A Coder's Worst Nightmare?](https://www.forbes.com/sites/quora/2014/12/05/what-is-a-coders-worst-nightmare/)
    * Poisoned compiler


* [Super Mario All-Stars + Super Mario World by SethBling, IsoFrieze in 11:55 - SGDQ 2022](https://www.youtube.com/watch?v=FlkWSqA4VFU) YouTube
    * Remote code execution


Cloud
-----

* [State of AWS Security: A Look Into Real-World AWS Environments](https://www.datadoghq.com/state-of-aws-security/)
    * IAM roles are complex and many organisations are vulnerable because they do not manage these credentials safely



---

* [EarSpy: Spying on Phone Calls via Ear Speaker Vibrations Captured by Accelerometer](https://www.securityweek.com/earspy-spying-phone-calls-ear-speaker-vibrations-captured-accelerometer)



[//begin]: # "Autogenerated link references for markdown compatibility"
[2fa]: 2fa.md "2 Factor Authentication"
[privacy]: privacy.md "Privacy"
[//end]: # "Autogenerated link references"
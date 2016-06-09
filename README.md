# freebsd-elantech

I got tired of not having proper support for my elantech touchpad under freebsd.  Luckily - I am not alone.

Code in this repo was originally suggested as a patch against 11 current in 2015, by Vladimir Kondratyev.  It was backported to 10 stable later than year by Rahael 'Kena' Poss.  I have taken these patches and implemented them against releng10.3 so that I can use it with freebsd 10.3.

Code presented compiles and provides support for elantech touchpads, as while they claim to be synaptics compatible: they actually use a slightly different protocol, and without this patch psm is fooled into treating them as a generic ps2 mouse.

Based on these patches:

https://lists.freebsd.org/pipermail/freebsd-amd64/2015-December/016199.html

https://lists.freebsd.org/pipermail/freebsd-mobile/2015-September/013327.html

Special Thanks to 
Vladimir Kondratyev
and
Raphael 'kena' Poss

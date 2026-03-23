---
id: a-practical-attack-on-des-circuitry
title: a practical attack on DES circuitry
type: writing
writing_type: rre-post
date: 1994-11-04
url: http://commons.somewhere.com:80/rre/1996/a.practical.attack.on.DE.html
coauthors: []
key_concepts: []
importance: 4
research_status: partial
tags:
  - forwarded-content
  - internet-culture
---




## Source

Automatically imported from: http://commons.somewhere.com:80/rre/1996/a.practical.attack.on.DE.html

## Content

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991006233110/http://www.somewhere.com/)

  

# a practical attack on DES circuitry

```
[What I find most interesting about this new attack on DES is that it
exploits the difference between the physical properties of logic circuitry
and the mathematical properties of logic formalisms.  This difference should
be obvious, except that computer work is full of linguistic ambiguities
that tend to conflate the difference between representation and reality.
Thus "logic" can mean either physical circuitry or mathematical formalisms.
Another example is "mouse", which can mean either the little box you slide
on the desktop with your hand or the little icon that moves around the
screen as a result.  Moreover, I'll bet that, if you read the source code
of a personal computer operating system, the data structure that stores
current parameters of the mouse is also called "mouse" or something very
similar.  Ross Anderson's home page is at www.cl.cam.ac.uk/users/rja14 ,
and it includes descriptions of much other work along these same lines.]

---

This message was forwarded through the Red Rock Eater News Service (RRE).
Send any replies to the original author, listed in the From: field below.
You are welcome to send the message along to others but please do not use
the "redirect" command.  For information on RRE, including instructions
for (un)subscribing, send an empty message to  rre-help@weber.ucsd.edu

---

Date: Sun, 3 Nov 1996 18:16:37 -0500
From: Ross Anderson <Ross.Anderson@cl.cam.ac.uk>
Subject: Announcement - Warning to Crypto and Banking Communities

		       A serious weakness of DES
		       Draft - 2nd November 1996

Abstract

Eli Biham and Adi Shamir recently pointed out that if an attacker can
induce unidirectional faults in key memory of cryptographic devices,
then keys could be extracted quickly. Although their attack is very
elegant, it is not practical against many fielded systems. For
example, inducing a single bit change in a DES key will cause a proper
implementation to return a key parity error.

However, when combined with Peter Gutman's recent work on memory
remanence, there are two very practical attacks. One of them allows
smartcard electronic wallet keys to be extracted with much less
expensive equipment than that currently used by pay-TV pirates; the
other yields an effective attack against fielded banking security
modules. These attacks show that a feature of DES that had long been
thought innocuous is actually a serious design error.

Introduction

In a research announcement of 30th October, Biham and Shamir point
out that if a cryptographic hardware module employes EEPROM for key
memory only, an opponent who can turn EEPROM values from `1' to `0'
with a small controlled probability (e.g., by applying UV light) might
cause a test input to be encrypted with a series of keys, each of
Hamming distance one from the next in the series, and ending with the
all zero key [1].

There are a number of reasons why their attack is not likely to work
against real systems. For example, the typical smartcard system has
several kilobytes of program code in EEPROM as well as typically two
to five DES keys. An undirected stress applied to such a card is more
likely to cause a program crash or an uninformative error than to
yield a ciphertext encrypted under a key at Hamming distance one from
a genuine key. Even if we only had to cause a hundred cards to fail
to get a single input for the Biham-Shamir attack, if we needed on
average 28 inputs to recover a DES key, then the number of cards
required could be O(100^28).

The situation is made still worse by the fact that DES keys have odd
parity, and a proper implementation will reject a key if any of its
bytes has even parity. So one would be reduced to looking for keys at
a Hamming distance of two rather than one. It is this objection that
inspired the following work.

A Modified Attack

My idea is to turn the DES key parity problem on its head and enable
parity to help rather than hinder the attack. Let us first consider
an opponent who can perform directed attacks on the chip. Reading the
contents of an EEPROM cell directly is difficult, and people who do
it for a living use focused ion beam workstations to modify the chip
[2]. However, it is trivial to set an EEPROM cell to the value of
your choice if you do not have to read it first; you only need two
microprobes. A 10mS 18V pulse from the cell's source to its control
gate will do the trick [3].

My modified attack therefore proceeds as follows. Set the first bit
of the EEPROM containing the target DES key to 1 (or 0, the choice
doesn't matter) and operate the device. If it still works, the keybit
was a 1. If you get a `key parity error' message, then the bit was
zero. Move on to the next bit; set it to 1 and see if this changes
the device's response (from encryption to error or vice versa).

This is a practical attack even on chips whose software we do not
know in detail, as many smartcard software writers seem to have
adopted a convention that the keys are located at the bottom end of
the EEPROM memory. It will also work with protocols that use
redundancy which we do not understand: we just change each key bit
back to its original value.

The use of predictable memory addresses for keys is not restricted to
smartcards; many banking security modules also keep keys at low
memory. I will now describe a related attack that extracts master
keys from these modules.

An Attack on Fielded Systems

In a brilliant Usenix paper [4], Peter Gutman described the
mechanisms that cause both static and dynamic RAM to `remember'
values that they have stored for a long period of time. A prudent
security engineer will ask what the effect of this is in the real
world.

I looked at an instance of a security module used in banking. This
security module has 12 pairs of DES master keys stored in low memory.
The device is tamper resistant in that power to the key memory is cut
when the box is opened for servicing (this is needed every few years
to change the battery). Keys are loaded into the device afterwards in
multiple components by trusted bank staff.

In this device, which dated from the late 1980's, the key values were
substantially intact on power-up. The number of bits in error was of
the order of 5-10%. I cannot give more accurate figures as I was not
permitted to copy down either the correct master key values, nor the
almost-correct values that had been `burned in' to the static RAM
chips. I am also not permitted to name the bank at which these modules
are installed, and it may not be prudent to name their manufacturer.

Nonetheless the crypto community should consider the consequences.

If each DES key is wrong by five bits, then the effort involved in
seaching for the 10 wrong bits in a double DES key might be thought
to be 112-choose-10 operations. Each operation would involve (a)
doing a 2-key 3DES decryption of a 64 bit PIN key whose enciphered
value is widely known to the bank's programmers (b) in the 2^{-8} of
cases where this result has odd parity, enciphering an account number
with this as a DES key to see if the (decimalised) result is the
corresponding PIN. The effort is 4 times 112-choose-10 DES operations

* about 2^50. But it would probably be cheaper to do a hardware

keysearch on the PIN key directly than to try to implement this more
complex 2^50 search in either hardware or software.

However, the bytewise nature of the DES key redundancy reduces the
effort by orders of magnitude. If no key byte has a double error,
then the effort is seven tries for each even parity byte observed, or
7^10 - about 2^28, which is easy. If there is one key byte with a
double error, the effort is 2^38, giving a search of 2^40 DES
operations - which is still feasible for an individual.

Conclusions

I have shown that the key parity in DES enables us to slash the cost
of real attacks on both old systems (banking security modules) and
new ones (electronic wallet smartcards).

I had already mentioned in [5] that a common fault in the driver
software for banking security modules was that `key parity error'
messages were often ignored rather than copied to the bank's security
manager to give warning of an attempted attack. This note shows that
key parity is even more serious than that.

The nature of DES key redundancy now appears to be a design error; it
would have been much better to calculate the redundancy on the whole
key. The 16 bit MAC used in the Clipper and Capstone chips is
preferable (although as shown in [6], 16 bits may not be enough to
prevent some protocol attacks).

The lesson for bankers is that existing security modules (and other
cryptographic devices) should be destroyed carefully at the end of
their working life.

The lesson for security engineers is that we should add key
redundancy, and the question of whether we can rely on a device's
eventual destruction, to the growing list of system parameters that
must be (a) explicitly considered during design and (b) examined
carefully when the product is being evaluated.

Bibliography

[1] ``The Next Stage of Differential Fault Analysis: How to break completely
unknown cryptosystems'', Eli Biham, Adi Shamir, October 30th, 1996

[2] ``Tamper Resistance - A Cautionary Note'', Ross Anderson, Markus Kuhn, to
appear at Usenix Electronic Commerce 96 (19th November)

[3] ``Hardwaresicherheit von Mikrochips in Chipkarten'', Osman Kocar,
Datenschutz und Datensicherheit v 20 no 7 (July 96) pp 421--424

[4] ``Secure Deletion of Data from Magnetic and Solid-State Memory'', Peter
Gutmann, Usenix Security 96 pp 77--89

[5] ``Why Cryptosystems Fail'', Ross Anderson, in Communications of the ACM v
7 no 11 (Nov 94) pp 32--40

[6] ``Protocol Failure in the Escrowed Encryption Standard'', Matt Blaze, in
Proceedings of the 2nd ACM Conference on Computer and Communications Security
(2-4 November 1994), ACM Press, pp 59--67
```

  

This web service brought to you by
[Somewhere.Com, LLC.](https://web.archive.org/web/19991006233110/http://www.somewhere.com/)
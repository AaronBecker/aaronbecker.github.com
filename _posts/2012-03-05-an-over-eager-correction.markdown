---
date: 2012-03-05 15:39 PM
title: An Over-Eager Correction
source: 
layout: post
---

This weekend I was listening to the most recent episode of
[Hypercritical][], which covered a variety of topics on file systems.
John Siracusa was discussing block de-duplication in ZFS and said that
when the file system sees that two blocks have the same checksum, it
knows that the blocks' contents are the same. I immediately thought "No!
Of course the number of possible checksum values is vastly smaller than
the number of distinct blocks, so collisions are possible and the file
system has to check and make sure that the blocks are actually the
same." Of course, as a Hypercritical listener I am eager to pick nits,
so I resolved to send in a correction.

Fortunately, I decided to do a little research first. I imagined that
ZFS must use a simple checksum like [CRC][] so that computing checksums
is as fast as possible. In fact, as I learned on [ZFS developer Jeff
Bonwick's blog](https://blogs.oracle.com/bonwick/entry/zfs_dedup), it
uses the crytographic hash [SHA1][], which has no known collisions. Of
course, collisions still exist, but the odds of encountering one is much
smaller than the odds that your file system will be corrupted by a freak
shower of cosmic rays. There is a ZFS option to use a cheaper hash and
do verification when checksums match, but the default is to use SHA1 and
do no checking.

So, I expected to write Jonn a note saying "You weren't quite right, and
the situation is more complicated than what you described on the show".
The actual situation is more like "You were exactly right, but there's
some hidden depth here". Which I'm sure is true of almost everything
that he covered on the show. There's not enough time to cover everything
to that level of detail, even if people were interested in it. But after
finding all this out, I decided to go ahead and write this all up
anyway, if for no other reason than to document the importance of doing
a little research to keep your foot out of your mouth.

[Hypercritical]: http://5by5.tv/hypercritical
[CRC]: http://en.wikipedia.org/wiki/Cyclic_redundancy_check
[SHA1]: http://en.wikipedia.org/wiki/SHA-1
